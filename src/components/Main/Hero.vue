<script setup>
    import hero from "@/assets/hero.png";
</script>

<template>
    <div
        class="container flex flex-col items-center justify-center px-3 py-4 text-white sm:mx-auto sm:flex-row sm:p-12"
    >
        <div class="space-y-5 sm:max-w-md">
            <h1 class="text-bold md:2xl text-xl lg:text-3xl">
                Hi! My name is <span class="text-purple-400">Yaroslav</span> and I'm
                <span class="text-purple-400">front-end developer</span>
            </h1>
            <p class="text-base text-slate-400">
                I craft responsive websites where technologies meet creativity
            </p>
            <button
                class="rounded-sm px-4 py-1 ring-1 ring-purple-500 duration-300 ease-in-out hover:bg-purple-500 hover:ring-0 active:scale-95"
            >
                Contact me!
            </button>
        </div>
        <div class="space-y-5 sm:max-w-md">
            <img
                :src="hero"
                alt="Cartoon Yaroslav programming"
                class="mx-auto w-[360px] object-cover sm:w-[460px]"
            />
            <div class="flex items-center gap-x-2 border px-2 py-1">
                <i class="fa-solid fa-square text-lg text-green-500"></i>
                <p class="text-sm md:text-base lg:text-lg">
                    Currently available for job opportunities
                </p>
            </div>
        </div>
    </div>
</template>
