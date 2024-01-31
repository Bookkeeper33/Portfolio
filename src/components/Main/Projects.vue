<script setup>
    import ProjectCard from "@/components/UI/ProjectCard.vue";
    import weatherApp from "@/assets/projects/weather-app.png";
    import todoApp from "@/assets/projects/todo.png";
    import restaurant from "@/assets/projects/restaurant.png";
    import brewery from "@/assets/projects/brewery.png";
    import sketch from "@/assets/projects/etch-a-sketch.png";
    import library from "@/assets/projects/library.png";

    const projects = [
        {
            name: "Weather App",
            description: "Weather Tracking app from Odin Project",
            img: weatherApp,
            techStack: ["HTML/CSS", "JavaScript", "Webpack"],
            code: "https://github.com/Bookkeeper33/Weather-App",
            preview: "https://bookkeeper33.github.io/Weather-App/",
        },
        {
            name: "To-Do App",
            description: "Task tracker app",
            img: todoApp,
            techStack: ["HTML/CSS", "JavaScript", "Webpack"],
            code: "https://github.com/Bookkeeper33/ToDo_app",
            preview: "https://bookkeeper33.github.io/ToDo_app/",
        },
        {
            name: "Restaurant Web Page",
            description: "Entire web page generated with JS.",
            img: restaurant,
            techStack: ["HTML/CSS", "JavaScript", "Webpack"],
            code: "https://github.com/Bookkeeper33/Restaurant_Page-Odin-",
            preview: "https://bookkeeper33.github.io/Restaurant_Page-Odin-/",
        },
        {
            name: "Beer App",
            description: "Beer collection catalogue with one random beer",
            img: brewery,
            techStack: ["React.js", "TypeScript", "Next.js", "Bootstrap"],
            code: "https://github.com/Bookkeeper33/BeerApp",
            preview: "https://app-brewery-test.vercel.app/",
        },
        {
            name: "Etch-a-Sketch",
            description: "An interactive sketchpad",
            img: sketch,
            techStack: ["HTML/CSS", "JavaScript"],
            code: "https://github.com/Bookkeeper33/-Etch-a-Sketch",
            preview: "https://bookkeeper33.github.io/-Etch-a-Sketch/",
        },
        {
            name: "Pocket Library",
            description: "Library application to store your favorite books and track them",
            img: library,
            techStack: ["HTML/CSS", "JavaScript"],
            code: "https://github.com/Bookkeeper33/Library/",
            preview: "https://bookkeeper33.github.io/Library/",
        },
    ];
</script>

<template>
    <section id="projects" class="w-full px-3 py-4 text-white sm:p-10">
        <div class="flex items-center justify-between md:container md:mx-auto">
            <div class="flex flex-auto items-center">
                <i class="fa-solid fa-hashtag text-xl text-purple-300"></i>
                <h2 class="text-lg sm:text-2xl">projects</h2>
            </div>
            <a href="https://github.com/Bookkeeper33?tab=repositories" target="_blank">
                <button class="group">
                    View all<i
                        class="fa-solid fa-angles-right ml-1 text-sm duration-300 ease-in-out group-hover:translate-x-1 group-hover:text-purple-500"
                    ></i>
                </button>
            </a>
        </div>
        <div
            class="mt-5 flex flex-col items-center gap-y-5 md:container sm:grid sm:grid-cols-2 sm:gap-x-5 md:mx-auto md:justify-items-center lg:grid lg:grid-cols-3"
        >
            <ProjectCard
                v-for="project in projects"
                :project-name="project.name"
                :description="project.description"
                :img="project.img"
                :tech-stack="project.techStack"
                :code="project.code"
                :preview="project.preview"
            />
        </div>
    </section>
</template>
