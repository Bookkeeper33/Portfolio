<script setup>
    const props = defineProps({
        skill: Object,
    });
</script>

<template>
    <div class="w-full rounded-sm border-2 border-gray-400 *:px-2 *:py-1 sm:max-w-[360px]">
        <h3 class="text-zinc-2s00 border-b-2 border-b-gray-400 text-base font-bold sm:text-lg">
            {{ skill.title }}
        </h3>
        <p class="text-sm text-slate-300 sm:text-base">{{ skill.technologies.join(", ") }}</p>
    </div>
</template>
