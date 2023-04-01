<template>
    <div class='flex items-center rounded-md bg-white w-full h-full pr-20 relative'>
        <div class="w-2/5 overflow-hidden text-[2.5em] relative z-[2]">
          We are <span class="gradientText">India's</span> <br/> 
          largest network of <br/>
          <span class="gradientText">micro</span>-influencers
        </div>
        <div class="w-3/5 relative">
          <div class="heading text-2xl">Offering best influencers <span class="font-bold  gradientText">RRRates</span></div>
          <div class="grid grid-cols-3 gap-8 my-10 relative z-10">
            <figure class="rounded-full h-[50vh] overflow-hidden hover:scale-150 cursor-pointer transition duration-700 ease-in-out border-4 border-white">
              <img src="../../assets/influencer1.jpg" alt="" class="w-full h-full object-cover">
            </figure>
            <figure class="rounded-full h-[50vh] overflow-hidden hover:scale-150 cursor-pointer transition duration-700 ease-in-out border-4 border-white">
              <img src="../../assets/influencer2.png" alt="" class="w-full h-full object-cover">
            </figure>
            <figure class="rounded-full h-[50vh] overflow-hidden hover:scale-150 cursor-pointer transition duration-700 ease-in-out border-4 border-white">
              <img src="../../assets/influencer3.png" alt="" class="h-full w-full object-cover">
            </figure>
          </div>
          <div class="bottom-text text-2xl">for your influencer campaign to go <br/> <span class="gradientText font-bold">#NatuNatu</span></div>
          <img src="../../assets/icon2.svg" alt="arrow-icon" class="absolute right-0 -bottom-[20%] w-[70vw]">
        </div>
        <!-- vectors -->
        <img src="../../assets/arrowIcon.svg" alt="arrow-icon" class="absolute left-0 -bottom-[25vh] w-[36vw] z-[1]">
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