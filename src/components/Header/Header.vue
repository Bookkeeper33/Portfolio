<script setup>
    import { ref } from "vue";
    import Signal from "../../assets/icons/Signal.vue";
    import Burger from "../../assets/icons/Burger.vue";
    import Mark from "../../assets/icons/Mark.vue";

    import Navigation from "./Navigation.vue";

    const isOpen = ref(false);

    const toggleBurger = () => {
        isOpen.value = !isOpen.value;
    };
</script>

<template>
    <header class="flex justify-center px-3 py-5 text-base sm:text-xl">
        <div class="container flex flex-col items-center justify-between gap-2 gap-y-5 sm:flex-row">
            <div class="flex w-full justify-between gap-x-2 text-white sm:w-auto">
                <span class="flex items-center justify-center gap-x-2"><Signal />Bookkeeper</span>
                <button
                    @click="toggleBurger()"
                    aria-label="Toggle navigation menu"
                    class="block text-white transition-transform active:scale-75 sm:hidden"
                >
                    <Burger v-if="!isOpen" />
                    <Mark v-else />
                </button>
            </div>

            <Navigation :class="{ hidden: !isOpen }" class="sm:block" />
        </div>
    </header>
</template>
