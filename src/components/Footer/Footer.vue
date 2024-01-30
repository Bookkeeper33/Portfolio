<script setup>
    import { ref } from "vue";

    const currentYear = ref(new Date().getFullYear());
</script>

<template>
    <footer class="flex justify-center border-t border-t-purple-400 px-3 py-4 sm:p-4">
        <div
            class="container flex flex-col items-center gap-y-3 text-white sm:grid sm:grid-cols-2 sm:grid-rows-1"
        >
            <div class="self-start sm:justify-self-start">
                <h2 class="mb-3 text-lg font-bold sm:text-xl">Contact me</h2>
                <address class="flex items-center gap-x-2">
                    <i
                        class="fa-regular fa-envelope cursor-pointer text-lg text-purple-300 duration-300 ease-in-out hover:-translate-y-2 hover:text-purple-500 sm:text-2xl"
                    ></i>
                    <a
                        href="mailto:yaroslavmuller98@gmail.com"
                        class="text-sm duration-300 ease-out hover:opacity-80 sm:text-base"
                        >yaroslavmuller98@gmail.com
                    </a>
                </address>
            </div>
            <div class="min-w-[250px] self-start sm:justify-self-end">
                <h2 class="mb-3 text-lg font-bold sm:text-right sm:text-xl">Media</h2>
                <ul class="flex gap-x-5 sm:justify-end">
                    <li>
                        <a
                            href="https://www.linkedin.com/in/bookkeeper33/"
                            target="_blank"
                            aria-label="social network, open new tab"
                            ><i
                                class="fa-brands fa-linkedin text-lg text-purple-300 duration-300 ease-in-out hover:text-purple-500 sm:text-2xl"
                            ></i
                        ></a>
                    </li>
                    <li>
                        <a
                            href="https://github.com/Bookkeeper33"
                            target="_blank"
                            aria-label="social network, open new tab"
                            ><i
                                class="fa-brands fa-github text-lg text-purple-300 duration-300 ease-in-out hover:text-purple-500 sm:text-2xl"
                            ></i
                        ></a>
                    </li>
                    <li>
                        <a
                            href="https://t.me/melnyk_ya"
                            target="_blank"
                            aria-label="social network, open new tab"
                            ><i
                                class="fa-brands fa-telegram text-lg text-purple-300 duration-300 ease-in-out hover:text-purple-500 sm:text-2xl"
                            ></i
                        ></a>
                    </li>
                </ul>
            </div>
            <div
                class="col-span-2 justify-self-center text-xs italic max-[300px]:text-center sm:text-sm"
            >
                &copy; Copyright {{ currentYear }}. Made by Bookkeeper
            </div>
        </div>
    </footer>
</template>
