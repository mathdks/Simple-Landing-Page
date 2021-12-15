<template>
    <section class="bg-black relative">
        <div class="bg-fixed bg-black h-screen bg-cover flex hero-image bg-opacity-40" :style="{backgroundImage: 'url('+require('../assets/tharali-hero.jpg')+')'}">
            <div class="flex flex-col md:flex-row absolute justify-around items-center h-full w-full">
                <div class="z-10 h-64 w-5/6">
                    <span>
                        <h1 class="text-4xl font-bold">Ajudamos você a <span class="text-yellow-600">construir o seu sonho</span>.</h1>
                        <h2 class="text-xl font-semibold text-white">Com tranquilidade, eficiência e qualidade.</h2>
                    </span>
                    <div class="py-5 flex flex-row">
                        <button v-scroll-to="'#about'" type="button" class="focus:outline-none rounded-l-full p-3 bg-yellow-600 font-bold text-lg text-white w-52">
                        Saiba mais
                        </button>
                        <button v-scroll-to="'#contact'" type="button" class="focus:outline-none rounded-r-full p-3 bg-green-600 font-bold text-lg text-white w-52">
                        Pedir orçamento
                        </button>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<script>
export default {

}
</script>

<style>
.hero-image::after {
  display: block;
  position: absolute;
  background-image: linear-gradient(to bottom, rgba(255, 255, 255, 0) 0, #000 100%);
  bottom: 0;
  left:0;
  right:0;
  height: 100vh;
  width: 100%;
  content: '';
}
</style>