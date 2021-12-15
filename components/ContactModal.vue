<template>
  <div>
    <button @click="toggleModal()" type="button" class="focus:outline-none rounded-full bg-green-500 w-40 p-2 font-semibold text-lg text-white">
        Pedir Orçamento
    </button>
    <div v-if="showModal" class="overflow-y-auto relative z-50">
      <div class="relative w-full mx-auto h-96">
        <!--content-->
        <div class="border-0 rounded-lg shadow-lg relative flex flex-col w-full bg-white outline-none focus:outline-none">
          <!--header-->
          <div class="flex items-start justify-between p-5 border-b border-solid border-blueGray-200 rounded-t">
            <h3 class="text-3xl font-semibold text-center">
              Pedido de Orçamento
            </h3>
            <button class="p-1 ml-auto bg-transparent border-0 text-black float-right text-3xl leading-none font-semibold outline-none focus:outline-none" @click="toggleModal()">
              <span class="bg-transparent text-black h-6 w-6 text-2xl block outline-none focus:outline-none">
                ×
              </span>
            </button>
          </div>
          <!--body-->
          <div class="px-5">
            <Contato />
          </div>
        </div>
      </div>
    </div>
    <div @click="toggleModal()" v-if="showModal" class="opacity-70 fixed inset-0 z-40 bg-black"></div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      showModal: false
    }
  },
  methods: {
    toggleModal: function(){
      this.showModal = !this.showModal;
    }
  }
}
</script>