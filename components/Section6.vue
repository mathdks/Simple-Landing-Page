<template>
    <section>
        <div class="items-center w-full md:px-20 p-8 bg-gradient-to-b from-yellow-100 via-white h-screen flex">
            <div class="relative md:h-4/5 h-full w-full bg-white rounded-xl">
                    <h1 class="w-full absolute p-5 text-center text-transparent font-black text-4xl bg-clip-text bg-gradient-to-b from-yellow-700 to-yellow-400">
                        Entre em Contato
                    </h1>
                <div class="h-full flex flex-col place-items-center place-content-center text-center">
                    <div class="text-justify md:w-1/4 w-4/5">

                        <p>A casa que você sempre sonhou está cada vez mais próxima de se tornar uma realidade.<br><br></p>
                        <strong><p class="text-lg">Entre em contato agora e dê mais um passo rumo à realização desse sonho.</p></strong>
                        
                    </div>
                    <div class="flex p-5">
                            <ContactModal />
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