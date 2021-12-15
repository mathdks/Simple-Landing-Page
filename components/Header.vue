<template>
    <div class="sticky top-0 z-40 shadow-sm">
        <nav id="nav" class="bg-black">
            <div class="max-w-7xl mx-auto px-2 sm:px-6 lg:px-8">
                <div class="relative flex items-center justify-between h-24">
                    <MobileMenu />
                    <div class="flex-1 flex items-center justify-center">
                        <div class="flex-shrink-0 flex items-center">
                            <NuxtLink to="/" class="flex place-items-center px-10 py-2">
                                <img class="block lg:hidden h-16 w-auto" src="../assets/logo-tharali.png" alt="Tharali Engenharia">
                                <img class="hidden lg:block h-20 w-auto" src="../assets/logo-tharali.png" alt="Tharali Engenharia">
                            </NuxtLink>
                        </div>
                    </div>
                </div>
            </div>
        </nav>
    </div>
</template>

<script>
    export default {
        methods: {
            dark(){
            }
        }
    }
</script>
