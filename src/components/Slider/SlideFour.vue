<template>
    <div class='flex w-full items-center rounded-md h-[calc(100vh-60px)] overflow-hidden'>
        <div class='hero-text text-left w-full relative h-full flex items-center'>
            <div class="blobStill">
                <svg xmlns:xlink="http://www.w3.org/1999/xlink" version="1.1" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 310 350">
                    <path d="M156.4,339.5c31.8-2.5,59.4-26.8,80.2-48.5c28.3-29.5,40.5-47,56.1-85.1c14-34.3,20.7-75.6,2.3-111  c-18.1-34.8-55.7-58-90.4-72.3c-11.7-4.8-24.1-8.8-36.8-11.5l-0.9-0.9l-0.6,0.6c-27.7-5.8-56.6-6-82.4,3c-38.8,13.6-64,48.8-66.8,90.3c-3,43.9,17.8,88.3,33.7,128.8c5.3,13.5,10.4,27.1,14.9,40.9C77.5,309.9,111,343,156.4,339.5z"/>
                </svg>
            </div>
            <div class="px-12">
                <div class='text-[2.8em] font-bold relative'>"From Concept to <span class="text-red-600">creation</span>"</div>
                <p class="text-3xl">Let our designer cater your <br> UI/UX/branding/motion graphics</p>
            </div>
        </div>
        <div class="w-full">
            <video src="../../assets/UIUX.mp4" autoplay muted playsinline loop class="object-contain"></video>
        </div>
    </div>
</template>


<style scoped>
.blobStill {
    position: absolute;
    top: 0;
    left: -12em;
    width: 38vmax;
    z-index: -1;
    animation: move 10s ease-in-out infinite;
    fill: #fc4a1a;  /* fallback for old browsers */
    fill: -webkit-linear-gradient(to right, #f7b733, #fc4a1a);  /* Chrome 10-25, Safari 5.1-6 */
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