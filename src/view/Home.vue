<script setup>
    import { ref } from "vue";
    import { useIntersectionObserver } from "@vueuse/core";
    import Header from "@/components/Header/Header.vue";
    import Footer from "@/components/Footer/Footer.vue";
    import Hero from "@/components/Main/Hero.vue";
    import Projects from "@/components/Main/Projects.vue";
    import Skills from "@/components/Main/Skills.vue";
    import About from "@/components/Main/About.vue";
    import Contact from "@/components/Main/Contact.vue";

    const hero = ref(null);
    const isVisible = ref(true);

    const { stop } = useIntersectionObserver(
        hero,
        ([{ isIntersecting }], observerElement) => {
            isVisible.value = isIntersecting;
        },
        {
            rootMargin: "-30% 0px 0px 0px",
        }
    );
</script>

<template>
    <Header
        class="text-gray-100"
        :class="{
            'fixed left-0 right-0 top-0 bg-slate-800 shadow-sm shadow-slate-800': !isVisible,
        }"
    />
    <main class="flex flex-auto flex-col gap-y-5 text-white">
        <Hero ref="hero" />
        <Projects />
        <Skills />
        <About />
        <Contact />
    </main>
    <Footer />
</template>
