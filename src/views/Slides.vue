<template>
    <div class="h-[calc(100vh-60px)] relative">
        <!-- <carousel :items-to-show="1" :autoplay="5000" :wrap-around="true"> -->
        <carousel :items-to-show="1" :wrap-around="true">
            <slide v-for="slide in slides" :key="slide">
                <component :is="slide" />
            </slide>

            <template #addons>
                <navigation />
                <!-- <pagination /> -->
            </template>
        </carousel>

        <!-- <div class="scroll-btn absolute bottom-4 ml-[50%] translate-x-[-50%] flex flex-col justify-center items-center text-zinc-700">
            Scroll down <br/>
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-5 h-5 animate-bounce text-zinc-800">
                <path stroke-linecap="round" stroke-linejoin="round" d="M19.5 13.5L12 21m0 0l-7.5-7.5M12 21V3" />
            </svg>
        </div> -->
    </div>


</template>

<script setup>
    import 'vue3-carousel/dist/carousel.css'
    import { Carousel, Slide, Pagination, Navigation } from 'vue3-carousel'
    import { ref, shallowRef } from 'vue';
    import SlideOne from "../components/Slider/SlideOne.vue"
    import SlideTwo from "../components/Slider/SlideTwo.vue"
    import SlideThree from "../components/Slider/SlideThree.vue"
    import SlideFour from "../components/Slider/SlideFour.vue"
    import SlideFive from "../components/Slider/SlideFive.vue"

    const slides = shallowRef([
        SlideOne, SlideTwo, SlideThree, SlideFour, SlideFive
    ])

</script>