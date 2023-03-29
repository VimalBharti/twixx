<template>
    <div class='flex items-center rounded-md w-full h-[calc(100vh-60px)] overflow-hidden'>
        <video 
            src="../../assets/content-marketing.mp4" 
            class="w-full object-contain h-full"
            autoplay muted playsinline loop
        ></video>
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