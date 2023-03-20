<template>
    <div class="flex w-full gap-8 min-h-screen h-full py-10 overflow-hidden">
        <div class="w-2/5 flex flex-col pt-32 items-center relative">
            <div class="relative z-10">
        
                <div class="text-[4em] font-bold leading-[1.2em]">Our <br/> Services</div>
            </div>
            <svg xmlns:xlink="http://www.w3.org/1999/xlink" version="1.1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 310 350" class="blobService">
                <path d="M156.4,339.5c31.8-2.5,59.4-26.8,80.2-48.5c28.3-29.5,40.5-47,56.1-85.1c14-34.3,20.7-75.6,2.3-111  c-18.1-34.8-55.7-58-90.4-72.3c-11.7-4.8-24.1-8.8-36.8-11.5l-0.9-0.9l-0.6,0.6c-27.7-5.8-56.6-6-82.4,3c-38.8,13.6-64,48.8-66.8,90.3c-3,43.9,17.8,88.3,33.7,128.8c5.3,13.5,10.4,27.1,14.9,40.9C77.5,309.9,111,343,156.4,339.5z"/>
            </svg>
        </div>
        <div class="w-full px-6">
            <h2 class="text-[2.5em] font-medium">We make your brand more appealing</h2>
            <p class="mt-3">At Twixx, we offer a range of services to help you grow your business.</p>
            <!-- <hr class="my-8" /> -->
            <div class="gallery grid grid-cols-3 gap-6 mt-10">
                <div class="flex flex-col items-center gap-3 border rounded-xl py-10">
                    <img src="../assets/content-marketing.png" alt="" class="h-28 w-full object-contain">
                    <div>Content Marketing</div>
                </div>
                <div class="flex flex-col items-center gap-3 border rounded-xl py-10">
                    <img src="../assets/Graphic.png" alt="" class="h-28 w-full object-contain">
                    <div>Graphic</div>
                </div>
                <div class="flex flex-col items-center gap-3 border rounded-xl py-10">
                    <img src="../assets/influencer-marketing.png" alt="" class="h-28 w-full object-contain">
                    <div>Influencer Marketing</div>
                </div>
                <div class="flex flex-col items-center gap-3 border rounded-xl py-10">
                    <img src="../assets/Logo-Designing.png" alt="" class="h-28 w-full object-contain">
                    <div>Logo Designing</div>
                </div>
                <div class="flex flex-col items-center gap-3 border rounded-xl py-10">
                    <img src="../assets/SEO.png" alt="" class="h-28 w-full object-contain">
                    <div>Search Engine Optimization</div>
                </div>
                <div class="flex flex-col items-center gap-3 border rounded-xl py-10">
                    <img src="../assets/social-media-marketing.png" alt="" class="h-28 w-full object-contain">
                    <div>Social Media Marketing</div>
                </div>
            </div>
        </div>

        <!-- Scroll-btn -->
        <div class="scroll-btn absolute bottom-4 ml-[50%] translate-x-[-50%] flex flex-col justify-center items-center text-zinc-700">
            Scroll down <br/>
            <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-5 h-5 animate-bounce text-zinc-800">
                <path stroke-linecap="round" stroke-linejoin="round" d="M19.5 13.5L12 21m0 0l-7.5-7.5M12 21V3" />
            </svg>
        </div>
    </div>
</template>


<script setup>
    import 'vue3-carousel/dist/carousel.css'
    import { Carousel, Slide, Pagination, Navigation } from 'vue3-carousel'
    import { ref, shallowRef } from 'vue';

    const images = ref([
        'https://www.schbang.com/wp-content/themes/salient/img/new-home-images/Digital-Content-Creation-and-SEO.svg',
        'https://www.schbang.com/wp-content/themes/salient/img/new-home-images/E-commerce-Strategy-and-Execution.svg',
        'https://www.schbang.com/wp-content/themes/salient/img/new-home-images/Influencer-Relationship-Celebrity-Management-&-PR.svg',
        'https://www.schbang.com/',
        'https://www.schbang.com/wp-content/themes/salient/img/new-home-images/Integrated-Marketing-Solutions.svg',
        'https://www.schbang.com/wp-content/themes/salient/img/new-home-images/Media-Planning-and-Buying.svg',
        'https://www.schbang.com/wp-content/themes/salient/img/new-home-images/Technology-and-Design.svg'
    ])

</script>

<style scoped>
.blobService {
    position: absolute;
    top: 0em;
    left: -12em;
    /* z-index: -1; */
    width: 28vmax;
    animation: move 10s ease-in-out infinite;
    fill: #820dd0;  /* fallback for old browsers */
    fill: -webkit-linear-gradient(to right, #f7b733, #820dd0);  /* Chrome 10-25, Safari 5.1-6 */
    fill: linear-gradient(to right, #f7b733, #fc4a1a); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */

}
@keyframes move {
  0%   { transform: scale(1) translate(2px, 6px); }
  38%  { transform: scale(1) translate(5vw, 5vh) rotate(5deg); }
  40%  { transform: scale(1) translate(5vw, 5vh) rotate(5deg); }
  78%  { transform: scale(1) translate(0vw, 5vh) rotate(-1deg); }
  80%  { transform: scale(1) translate(0vw, 5vh) rotate(-1deg); }
  100% { transform: scale(1) translate(2px, 6px); }
}
</style>