<script setup>
    import Hashtag from "../../assets/icons/Hashtag.vue";
</script>

<template>
    <nav>
        <ul class="flex flex-col gap-y-2 text-white sm:flex-row sm:gap-x-10">
            <li class="flex justify-center gap-0">
                <span class="self-center"><Hashtag class="text-purple-500" /></span>
                <a href="#" class="transition-opacity duration-300 hover:opacity-70">about</a>
            </li>
            <li class="flex justify-center gap-0">
                <span class="self-center"><Hashtag class="text-purple-500" /></span>
                <a href="#" class="transition-opacity duration-300 hover:opacity-70">projects</a>
            </li>
            <li class="flex justify-center gap-0">
                <span class="self-center"><Hashtag class="text-purple-500" /></span>
                <a href="#" class="transition-opacity duration-300 hover:opacity-70">contacts</a>
            </li>
        </ul>
    </nav>
</template>
