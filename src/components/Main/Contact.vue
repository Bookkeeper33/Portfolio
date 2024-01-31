<template>
    <section id="contacts" class="w-full px-3 py-4 text-white sm:p-10">
        <div class="container mx-auto flex items-center">
            <i class="fa-solid fa-hashtag text-xl text-purple-300"></i>
            <h2 class="text-lg sm:text-2xl">contacts</h2>
        </div>
        <div
            class="container mx-auto mt-5 flex flex-col items-start gap-3 text-white sm:justify-between md:flex-row"
        >
            <p class="text-pretty text-gray-400 antialiased">
                I'm interested in
                <span class="text-purple-400">remote front-end developer opportunities</span>.
                However, if you have other request or question, don't hesitate to
                <span class="text-purple-400">contact me</span>!
            </p>
            <div
                class="flex w-full flex-col gap-3 sm:flex-row sm:justify-between sm:gap-5 md:justify-end md:gap-x-7"
            >
                <address class="not-italic">
                    <h3
                        class="mb-3 text-base font-bold sm:text-left sm:text-lg md:text-right md:text-xl"
                    >
                        Mail
                    </h3>
                    <span class="flex items-center gap-x-2">
                        <i
                            class="fa-regular fa-envelope cursor-pointer text-lg text-purple-300 duration-300 ease-in-out hover:-translate-y-2 hover:text-purple-500 sm:text-2xl"
                        ></i>
                        <a
                            href="mailto:yarko12@gmail.com"
                            aria-label="personal email"
                            class="text-sm duration-300 ease-out hover:opacity-80 sm:text-base"
                            >yarko12@gmail.com
                        </a>
                    </span>
                </address>

                <div>
                    <h3 class="mb-3 text-base font-bold sm:text-right sm:text-lg md:text-xl">
                        Media
                    </h3>
                    <ul class="flex gap-x-5 sm:justify-end">
                        <li>
                            <a
                                href="https://www.linkedin.com/in/bookkeeper33/"
                                target="_blank"
                                aria-label="LinkedIn, open new tab"
                                ><i
                                    class="fa-brands fa-linkedin text-lg text-purple-300 duration-300 ease-in-out hover:text-purple-500 sm:text-2xl"
                                ></i
                            ></a>
                        </li>
                        <li>
                            <a
                                href="https://github.com/Bookkeeper33"
                                target="_blank"
                                aria-label="github, open new tab"
                                ><i
                                    class="fa-brands fa-github text-lg text-purple-300 duration-300 ease-in-out hover:text-purple-500 sm:text-2xl"
                                ></i
                            ></a>
                        </li>
                        <li>
                            <a
                                href="https://t.me/melnyk_ya"
                                target="_blank"
                                aria-label="telegram, open new tab"
                                ><i
                                    class="fa-brands fa-telegram text-lg text-purple-300 duration-300 ease-in-out hover:text-purple-500 sm:text-2xl"
                                ></i
                            ></a>
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </section>
</template>
