<template>
    <section>
        <div class="items-center w-full md:px-20 p-8 bg-gradient-to-b from-yellow-500 via-yellow-400 to-yellow-300 h-screen flex">
            <div class="relative md:h-4/5 h-full w-full bg-white rounded-xl">
                <h1 class="w-full absolute p-5 text-center text-transparent font-black text-4xl bg-clip-text bg-gradient-to-b from-yellow-700 to-yellow-400">
                    Opinião dos Clientes
                </h1>
                <div class="h-full flex flex-col place-content-center">
                    <div class="flex">
                        <div class="h-80 md:h-full w-full">
                            <SliderMobile class="block sm:hidden" />
                            <Slider class="hidden sm:block" />
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
.flip-vertical {
    --transform-scale-y: -1;
}
</style>