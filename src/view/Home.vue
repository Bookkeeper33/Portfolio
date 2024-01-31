<script setup>
    import Header from "@/components/Header/Header.vue";
    import Footer from "@/components/Footer/Footer.vue";
    import Hero from "@/components/Main/Hero.vue";
    import Projects from "@/components/Main/Projects.vue";
    import Skills from "@/components/Main/Skills.vue";
    import About from "@/components/Main/About.vue";
    import Contact from "@/components/Main/Contact.vue";
</script>

<template>
    <Header />
    <main class="flex flex-auto flex-col gap-y-5 text-white">
        <Hero />
        <Projects />
        <Skills />
        <About />
        <Contact />
    </main>
    <Footer />
</template>
