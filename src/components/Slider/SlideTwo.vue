<template>
    <div class='flex items-center rounded-md bg-white w-full h-full'>
        <div class='hero-text text-left w-full dark:text-zinc-200 absolute flex items-center justify-center flex-col'>
            <div class='text-[4em] font-bold text-center'>
                India's largest network of <br/> 
                <div class="message"></div>
                influencers
            </div>
            <button class="bg-blue-600 text-white px-8 py-3 mt-10">Know More</button>
        </div>
        <video src="../../assets/micro.mp4" class="w-full h-[calc(100vh-60px)] object-cover" autoplay muted playsinline loop></video>
    </div>
</template>

<style scoped>
.message {
  color: #333;
}
.message::before{
    background-color: yellow;
    border-radius: 4px;
    animation: openclose 5s ease-in-out infinite;
    content: '';
    padding: 2px 16px;
    text-transform: uppercase;
}
@keyframes openclose {
  0% {
    width: 250px;
    content: 'nano'
  }
  25%{
    width: 0;
  }
  50% {
    width: 250px;
    content: 'micro'
  }
  75% {
    width: 0;
  }
  100% {
    width: 250px;
    content: 'macro'
  }
}
</style>