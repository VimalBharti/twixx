<template>
    <div class='flex items-center px-6 rounded-md w-full h-[calc(100vh-60px)] overflow-hidden'>
        <div class='hero-text text-left w-full text-zinc-800 px-12'>
            <div class='text-[3.5em] font-bold'>
                Content is the key
            </div>
            <p class="text-2xl">"We will create your story <br/> with our content"</p>
            <button class="bg-blue-600 text-white px-8 py-3 mt-12">Know More</button>
        </div>
        <div class="relative w-full h-full">
            <video 
                src="../../assets/content.mp4" 
                class="w-full object-contain h-full relative"
                autoplay muted playsinline loop
            ></video>
        </div>
    </div>
</template>


<style scoped>
.blob {
  position: absolute;
  top: 0;
  left: 0;
  fill: #023F92;
  width: 50vmax;
  z-index: -1;
  animation: move 10s ease-in-out infinite;
  transform-origin: 10% 10%;
}
@keyframes move {
  0%   { transform: scale(1)   translate(10px, -30px); }
  38%  { transform: scale(0.8, 1) translate(50vw, 10vh) rotate(60deg); }
  40%  { transform: scale(0.8, 1) translate(50vw, 10vh) rotate(60deg); }
  78%  { transform: scale(1.3) translate(0vw, 50vh) rotate(-5deg); }
  80%  { transform: scale(1.3) translate(0vw, 50vh) rotate(-5deg); }
  100% { transform: scale(1)   translate(10px, -10px); }
}
</style>