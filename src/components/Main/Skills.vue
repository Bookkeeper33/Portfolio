<script setup>
    import SkillCard from "@/components/UI/SkillCard.vue";

    const skills = [
        {
            title: "Core stack",
            technologies: ["JavaScript", "TypeScript", "HTML", "CSS"],
        },
        {
            title: "Frameworks",
            technologies: ["Vue.js", "React.js", "Nuxt.js", "Next.js", "Tailwindcss", "Bootstrap"],
        },
        {
            title: "Tools",
            technologies: ["VScode", "Git", "Webpack", "Vite", "Linux"],
        },
    ];
</script>

<template>
    <section class="w-full px-3 py-4 sm:p-10">
        <div class="container mx-auto flex items-center">
            <i class="fa-solid fa-hashtag text-xl text-purple-300"></i>
            <h2 class="text-lg sm:text-2xl">skills & <span class="text-purple-400">tools</span></h2>
        </div>
        <div
            class="container mx-auto mt-5 flex flex-col items-center gap-4 sm:flex-row sm:items-start sm:justify-center lg:justify-end"
        >
            <SkillCard v-for="skill in skills" :skill="skill" />
        </div>
    </section>
</template>
