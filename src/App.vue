<script setup>
  import OpenMenu from "./components/Icons/menu.vue"
  import Close from "./components/Icons/close.vue"
  import { ref } from "vue";

  const menuWindow = ref(false)

  const showMenu = () => {
      menuWindow.value = true
  }
</script>

<template>
  <div class="relative h-full">

      <nav class='w-full py-3 h-[60px] bg-transparent backdrop-blur-lg z-30 fixed top-0'>
          <div class='w-full px-6 flex justify-between mx-auto'>
              <div class='logo flex gap-3 items-center'>
                  <router-link to="/"><img src="/logo.png" alt="" class="w-24"></router-link>
              </div>
              <div class='flex items-center gap-2'>
                <Close v-if="menuWindow" class="w-8 h-8 hover:scale-150 transition duration-700 ease-in-out hover-scale-110 cursor-pointer text-white" @click="menuWindow = false" />
                <OpenMenu v-else class="w-8 h-8 cursor-pointer" @click="showMenu" />
              </div>
          </div>
      </nav>
      <!-- Menu window -->
      <section 
        class="z-[28] w-screen top-0 left-0 h-full fixed flex flex-col items-center justify-center gap-10 bg-gradient-to-tr from-indigo-500 via-purple-500 to-pink-500 text-white floatNavbScreen" 
        :style="menuWindow ? 'clip-path: circle(75%);' : 'clip-path: circle(0px at calc(100% - 45px) 45px);' "
        :data-dismiss="menuWindow">
          <a href="#about" class="uppercase text-[3em] font-bold hover:scale-150 transition duration-700 ease-in-out" @click="menuWindow = false">About</a>
          <a href="#service" class="uppercase text-[3em] font-bold hover:scale-150 transition duration-700 ease-in-out" @click="menuWindow = false">Service</a>
          <a href="#work" class="uppercase text-[3em] font-bold hover:scale-150 transition duration-700 ease-in-out" @click="menuWindow = false">Work</a>
          <a href="#contact" class="uppercase text-[3em] font-bold hover:scale-150 transition duration-700 ease-in-out" @click="menuWindow = false">Contact</a>
      </section>

    <main class="h-full mt-[60px]">
      <router-view></router-view>
    </main>
  </div>
</template>

<style scoped>
.floatNavbScreen{
  transition: all 0.5s ease-in-out;
}
</style>

