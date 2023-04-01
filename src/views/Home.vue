<template>
    <div class="bg-white">
        <Slides />
        <Service id="service" />
        <Work id="work" />
        <Contact id="contact" />

        <!-- footer -->
        <footer class="bg-white rounded-lg shadow py-2">
            <div class="w-full mx-auto max-w-screen-xl p-4 md:flex md:items-center md:justify-between">
            <span class="text-sm text-gray-500 sm:text-center dark:text-gray-400">© 2023 Twixx. All Rights Reserved.
            </span>
            <ul class="flex flex-wrap items-center mt-3 text-sm font-medium text-gray-500 dark:text-gray-400 sm:mt-0">
                <li>
                    <a href="#" class="mr-4 hover:underline md:mr-6 ">About</a>
                </li>
                <li>
                    <a href="#" class="mr-4 hover:underline md:mr-6">Privacy Policy</a>
                </li>
                <li>
                    <a href="#" class="mr-4 hover:underline md:mr-6">Work</a>
                </li>
                <li>
                    <a href="#" class="hover:underline">Contact</a>
                </li>
            </ul>
            </div>
        </footer>

    </div>
</template>

<script setup>
    import { ref } from 'vue';
    import Slides from '../views/Slides.vue'
    import Service from '../views/Service.vue'
    import Work from '../views/Work.vue'
    import Contact from '../views/Contact.vue'

</script>