<script setup>
    const props = defineProps({
        projectName: String,
        description: String,
        techStack: Array,
        img: String,
        code: String,
        preview: String,
    });
</script>

<template>
    <div class="rounded-sm border">
        <div>
            <img :src="img" alt="project picture" />
        </div>
        <div class="border-b border-t p-2 text-sm text-slate-400 sm:text-base md:text-lg">
            {{ techStack.join(", ") }}
        </div>
        <div class="flex flex-col p-2">
            <h3 class="text-base font-bold sm:text-lg md:text-xl">{{ projectName }}</h3>
            <p class="text-sm text-slate-400 md:text-base">{{ description }}</p>
            <div
                class="mx-auto mb-3 mt-5 flex flex-col gap-5 md:flex-row md:items-center md:justify-center"
            >
                <a :href="preview" target="_blank" aria-label="opens in new tab">
                    <button
                        class="w-full rounded-sm border-none px-7 py-1 text-sm ring-1 ring-purple-400 duration-300 ease-in-out hover:bg-purple-500 sm:text-base"
                    >
                        Live<i class="fa-solid fa-flask ml-1 text-xs sm:text-sm"></i>
                    </button>
                </a>
                <a :href="code" target="_blank" aria-label="opens in new tab">
                    <button
                        class="w-full rounded-sm border-none px-7 py-1 text-sm ring-1 ring-teal-500 duration-300 ease-in-out hover:bg-teal-500 sm:text-base"
                    >
                        Code<i class="fa-solid fa-code ml-1 text-xs sm:text-sm"></i>
                    </button>
                </a>
            </div>
        </div>
    </div>
</template>
