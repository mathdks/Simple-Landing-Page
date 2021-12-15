<template>
    <div>
        <div class="relative inset-y-0 left-0 flex items-center sm:hidden">
            <button @click="openMenu" type="button" class="inline-flex items-center justify-center p-2 rounded-md text-gray-400" aria-controls="mobile-menu" aria-expanded="false">
            <span class="sr-only">Menu</span>
            <svg :class="active ? 'hidden' : 'block'" class=" h-6 w-6" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor" aria-hidden="true">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
            </svg>
            <svg :class="active ? 'block' : 'hidden'" class=" h-6 w-6" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke="currentColor" aria-hidden="true">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12" />
            </svg>
            </button>
        </div>
        <div @click="closeMenu" v-show="active" :class="active ? 'block' : 'hidden'" class="block md:hidden w-full h-screen bg-transparent flex-grow absolute" id="mobile-menu">
            <div class="p-4 space-y-1 z-20 shadow bg-gray-800 text-center">
                <div>
                <NuxtLink to="/" class="text-indigo-300 px-3 py-2 text-lg font-medium">Início</NuxtLink>
                </div>
                <hr>
                <div class="m-3">
                    <p class="text-white text-lg font-medium">Receba o melhor conteúdo de valor.<br>Siga nossas redes sociais!</p>
                    <span class="pt-3 relative inline-flex">
                    <Social/>
                    <span class="flex absolute pt-3 h-3 w-3 top-0 right-0 -mt-1 -mr-1">
                    <span class="animate-ping opacity-75 rounded-full bg-red-500 inline-flex absolute w-full h-full"></span>
                    <span class="relative inline-flex rounded-full h-3 w-3 bg-red-600"></span>
                    </span>
                    </span>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        data() {
            return {
            active: false
            }
        },
        methods: {
            openMenu(){
                this.active = !this.active
            },
            closeMenu(){
                this.active = false
            }
        }
    }

</script>

<style>

</style>