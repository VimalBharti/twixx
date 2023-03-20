<template>
    <nav class='w-full py-3 h-[60px] border-b border-zinc-50 bg-white backdrop-blur-lg'>
        <div class='w-full px-6 flex justify-between mx-auto'>
            <div class='logo flex gap-3 items-center'>
                <!-- <router-link to="/">Twixx</router-link> -->
                <router-link to="/"><img src="/logo.png" alt=""></router-link>
            </div>
            <div class='flex items-center gap-2'>
                <OpenMenu class="w-8 h-8 cursor-pointer" @click="showMenu" />
            </div>
            <!-- Menu window -->
            <section class="fixed z-[60] w-full top-0 left-0 h-full bg-white/30 backdrop-blur-xl flex flex-col items-center justify-center gap-10" v-if="menuWindow" :data-dismiss="menuWindow">
                <Close class="w-12 h-12 hover:scale-150 transition duration-700 ease-in-out hover-scale-110 cursor-pointer" @click="menuWindow = false" />
                <a href="#about" class="uppercase text-[3em] font-bold hover:scale-150 transition duration-700 ease-in-out" @click="menuWindow = false">About</a>
                <a href="#service" class="uppercase text-[3em] font-bold hover:scale-150 transition duration-700 ease-in-out" @click="menuWindow = false">Service</a>
                <a href="#work" class="uppercase text-[3em] font-bold hover:scale-150 transition duration-700 ease-in-out" @click="menuWindow = false">Work</a>
                <a href="#contact" class="uppercase text-[3em] font-bold hover:scale-150 transition duration-700 ease-in-out" @click="menuWindow = false">Contact</a>
            </section>
        </div>
    </nav>
</template>

<script setup>
    import OpenMenu from "../components/Icons/menu.vue"
    import Close from "../components/Icons/close.vue"
    import { ref } from "vue";

    const menuWindow = ref(false)

    const showMenu = () => {
        menuWindow.value = true
    }
</script>