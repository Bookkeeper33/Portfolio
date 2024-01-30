<script setup>
    import yaroslav from "@/assets/me.png";
</script>

<template>
    <section class="w-full px-3 py-4 text-white sm:p-10">
        <div class="container mx-auto flex items-center">
            <i class="fa-solid fa-hashtag text-xl text-purple-300"></i>
            <h2 class="text-lg sm:text-2xl">about-<span class="text-purple-400">me</span></h2>
        </div>
        <div
            class="container flex flex-col-reverse items-center text-white sm:mx-auto sm:flex-row-reverse sm:items-start sm:justify-end"
        >
            <img
                :src="yaroslav"
                alt=""
                class="max-w-[320px] self-center max-[320px]:w-full md:max-w-[360px]"
            />
            <div
                class="mt-5 space-y-4 text-pretty text-gray-400 antialiased *:text-base sm:max-w-lg md:space-y-5 lg:space-y-8"
            >
                <p class="text-sm">Hello, i'm <span class="text-purple-400">Yaroslav</span>!</p>
                <p class="text-sm">
                    I'm self-taught <span class="text-purple-400">front-end developer</span> based
                    in Kyiv, Ukraine. Armed with a solid foundation in HTML, CSS, and JavaScript,
                    I've honed my skills through hands-on
                    <span class="text-purple-400">exploration</span> and
                    <span class="text-purple-400">experimentation</span>.
                </p>
                <p class="text-sm">
                    My journey into the world of front-end development has been marked by a series
                    of engaging pet projects that showcase my
                    <span class="text-purple-400">creativity</span> and
                    <span class="text-purple-400">problem-solving</span>
                    abilities. Since 2021, I have been engaging in self-study to gain a foundational
                    understanding of computer science.
                </p>
            </div>
        </div>
    </section>
</template>
