<template>
  <a @click="scrollTop" v-show="visible" class="fixed bottom-5 right-5">
    <button class="focus:outline-none shadow-md border md:border-0 bg-white transition duration-500 ease-in-out transform hover:-translate-y-1 hover:scale-110 mx-2 p-2 bg-gradient-to-b hover:from-yellow-300 rounded-full">
      <svg class="opacity-60 w-8 h-8 fill-current text-black" viewBox="0 0 24 24" xmlns="http://www.w3.org/2000/svg">
        <path d="M 4 12 l 1.41 1.41 L 11 7.83 V 20 h 2 V 7.83 l 5.58 5.59 L 20 12 l -8 -8 l -8 8 Z"></path>
      </svg>
    </button>
  </a>
</template>

<script>
export default {
  data () {
    return {
      visible: false
    }
  },
  methods: {
    scrollTop: function () {
      this.intervalId = setInterval(() => {
        if (window.pageYOffset === 0) {
          clearInterval(this.intervalId)
        }
        window.scroll(0, window.pageYOffset - 85)
      }, 20)
    },
    scrollListener: function (e) {
      this.visible = window.scrollY > 350
    }
  },
  mounted: function () {
    window.addEventListener('scroll', this.scrollListener)
  },
  beforeDestroy: function () {
    window.removeEventListener('scroll', this.scrollListener)
  }
}
</script>