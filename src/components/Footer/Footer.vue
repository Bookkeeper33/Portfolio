<script setup>
    import { ref } from "vue";

    const currentYear = ref(new Date().getFullYear());
</script>

<template>
    <footer class="flex justify-center px-3 py-4 sm:p-4">
        <div class="text-xs text-white max-[300px]:text-center sm:text-sm">
            &copy; Copyright {{ currentYear }}. Made by Bookkeeper
        </div>
    </footer>
</template>
