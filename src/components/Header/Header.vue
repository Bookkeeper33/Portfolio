<script setup>
    import { ref } from "vue";
    import Navigation from "./Navigation.vue";

    const isOpen = ref(false);

    const toggleBurger = () => {
        isOpen.value = !isOpen.value;
    };
</script>

<template>
    <header class="flex justify-center px-3 py-5 transition duration-500 ease-linear">
        <div class="container flex flex-col items-center justify-between gap-2 gap-y-5 md:flex-row">
            <div class="flex w-full justify-between gap-x-2 md:w-auto">
                <span
                    class="group flex cursor-pointer items-center justify-center text-lg font-bold sm:text-2xl"
                    tabindex="0"
                    ><i
                        class="fa-solid fa-hashtag text-xl text-purple-300 duration-300 ease-in-out group-hover:text-purple-500"
                    ></i
                    ><a href="#home">Bookkeeper</a></span
                >
                <button
                    @click="toggleBurger()"
                    aria-label="Toggle navigation menu"
                    class="block transition-transform active:scale-75 md:hidden"
                >
                    <i v-if="!isOpen" class="fa-solid fa-align-right text-2xl text-purple-300"></i>
                    <i v-else class="fa-solid fa-circle-xmark text-2xl text-purple-300"></i>
                </button>
            </div>

            <Navigation :class="{ hidden: !isOpen }" class="md:block" />
        </div>
    </header>
</template>
