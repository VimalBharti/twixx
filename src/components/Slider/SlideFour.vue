<template>
    <div class='flex w-full items-center rounded-md h-[calc(100vh-60px)] overflow-hidden'>
        <div class='hero-text text-left w-2/5 relative h-full flex items-center justify-center'>
            <div class='text-[3em] font-bold relative'>From <br/> Concept <br/> to <br/> <span class="gradientText">creation</span></div>
        </div>
        <div class="w-3/5 h-full bg-gradient-to-r from-[#F29C40] via-[#EB7BB1] to-[#877EBB] p-12">
            <div class="grid grid-cols-1 md:grid-cols-2 gap-6">
                <figure class="rounded-2xl object-cover h-full overflow-hidden cursor-pointer hover:scale-125 transition duration-700 ease-in-out relative group">
                    <img src="../../assets/UIUX.jpg" alt="website/ui/ux" class="h-full w-full">
                    <button class="bg-black/70 text-sm rounded-full py-3 px-8 uppercase left-[50%] -translate-x-[50%] absolute text-white bottom-4 group-hover:bg-white/90 group-hover:text-zinc-800 transition duration-700 ease-in-out">Website</button>
                </figure>
                <figure class="rounded-2xl object-cover h-full overflow-hidden cursor-pointer hover:scale-125 transition duration-700 ease-in-out relative group">
                    <img src="../../assets/illustration.png" alt="website/ui/ux" class="h-full w-full">
                    <button class="bg-black/70 text-sm rounded-full py-3 px-8 uppercase left-[50%] -translate-x-[50%] absolute text-white bottom-4 group-hover:bg-white/90 group-hover:text-zinc-800 transition duration-700 ease-in-out">Illustrations</button>
                </figure>
                <figure class="rounded-2xl object-cover h-full overflow-hidden cursor-pointer hover:scale-125 transition duration-700 ease-in-out relative group">
                    <img src="../../assets/logo.png" alt="website/ui/ux" class="h-full w-full">
                    <button class="bg-black/70 text-sm rounded-full py-3 px-8 uppercase left-[50%] -translate-x-[50%] absolute text-white bottom-4 group-hover:bg-white/90 group-hover:text-zinc-800 transition duration-700 ease-in-out">Logo</button>
                </figure>
                <figure class="rounded-2xl object-cover h-full overflow-hidden cursor-pointer hover:scale-125 transition duration-700 ease-in-out relative group">
                    <img src="../../assets/socialmedia.jpg" alt="website/ui/ux" class="h-full w-full">
                    <button class="bg-black/70 text-sm rounded-full py-3 px-8 uppercase left-[50%] -translate-x-[50%] absolute text-white bottom-4 group-hover:bg-white/90 group-hover:text-zinc-800 transition duration-700 ease-in-out">Social Media</button>
                </figure>
            </div>
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
    fill: transparent;

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