<template>
    <div class="text-center">
        <hr class="border-t-4 border-yellow-100">
        <hr class="border-t-4 border-yellow-200">
        <hr class="border-t-4 border-yellow-300">
        <hr class="border-t-4 border-yellow-400">
        <hr class="border-t-4 border-yellow-500">
        <footer class="bg-black p-8 sm:p-12 text-white">
            <div class="flex flex-col">
                <div class="flex justify-center">
                    <img class="w-72 items-center" src="../assets/logo-tharali.png" alt="Tharali Engenharia">
                </div>
                <div class="flex flex-col md:flex-row justify-around items-center pt-5">
                    <div class="flex flex-col">
                        <h2 class="font-bold text-lg text-yellow-500">A Tharali</h2>
                        <button v-scroll-to="'#about'" type="button" class="focus:outline-none text-white">
                        Sobre
                        </button>
                        <button v-scroll-to="'#services'" type="button" class="focus:outline-none text-white">
                        Serviços
                        </button>
                    </div>
                    <div class="flex flex-col">
                        <h2 class="font-bold text-lg text-yellow-500">Suporte</h2>
                        <button v-scroll-to="'#faq'" type="button" class="focus:outline-none text-white">
                        FAQ
                        </button>
                        <button v-scroll-to="'#contact'" type="button" class="focus:outline-none text-white">
                        Contato
                        </button>
                    </div>
                    <div class="flex flex-col">
                        <h2 class="font-bold text-lg text-yellow-500">Acompanhe</h2>
                        <Social class="flex flex-row pt-2"/>
                    </div>
                </div>
                <div class="text-sm pt-10">
                    <span class="dark:text-white">Feito com muito </span>
                    <span class="text-red-600 text-lg">&#x2764; </span>
                    <span class="dark:text-white">por </span>
                    <span class="dark:text-white font-bold">Tharali Engenharia</span><br>
                    <span class="dark:text-white"><strong>Desde 2020 fazendo o melhor por você!</strong></span>
                </div>
            </div>
        </footer>
    </div>
</template>