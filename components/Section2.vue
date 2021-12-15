<template>
    <section>
        <div class="bg-gradient-to-b from-yellow-900 via-yellow-800 to-yellow-700 h-screen flex">
            <div class="flex flex-col md:flex-row justify-around items-center h-full w-full md:px-20 p-8">
                <div class="md:h-4/5 h-full w-full bg-white rounded-xl">
                    <h1 class="p-5 text-center text-transparent font-black text-4xl bg-clip-text bg-gradient-to-b from-yellow-700 to-yellow-400">
                        Serviços disponíveis
                    </h1>
                    <div class="flex md:flex-row flex-col md:justify-around items-center">
                        <div class="md:h-72 md:w-72 hidden md:flex items-center">
                            <Eng />
                        </div>
                        <div>
                            <Services />
                        </div>
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

</style>