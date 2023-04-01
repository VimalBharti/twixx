<template>
    <section class="contactSection min-h-screen pt-12">
        <div class="flex gap-8 h-full p-12 w-full relative items-center max-w-6xl mx-auto">
            <div class="w-full flex flex-col justify-center">
                <div class="text-[2.6em] font-bold">Contact Us Today</div>
                <div class="text-lg">Learn more about how <span class="gradientText font-bold">TWIXX</span> can help you unleash your brand's potential and take your business to the next level</div>
                <div class="mt-8 rounded-xl shadow-xl bg-white py-6 px-8 flex gap-5 justify-start w-[60%]">
                    <button class="p-3 rounded-xl bg-gray-100"> 
                        <svg xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24" stroke-width="1.5" stroke="currentColor" class="w-6 h-6">
                            <path stroke-linecap="round" stroke-linejoin="round" d="M21.75 6.75v10.5a2.25 2.25 0 01-2.25 2.25h-15a2.25 2.25 0 01-2.25-2.25V6.75m19.5 0A2.25 2.25 0 0019.5 4.5h-15a2.25 2.25 0 00-2.25 2.25m19.5 0v.243a2.25 2.25 0 01-1.07 1.916l-7.5 4.615a2.25 2.25 0 01-2.36 0L3.32 8.91a2.25 2.25 0 01-1.07-1.916V6.75" />
                        </svg>
                    </button>   
                    <div>
                        <div class="">Mail me at</div>
                        <div class="gradientText font-bold">hello@twixx.com</div>
                    </div>
                </div>
            </div>
            <div class="w-2/3">
                <h2 class="font-bold text-2xl uppercase mb-3">Queries Here</h2>
                <div class="shadow-lg rounded-lg p-8 flex flex-col items-start bg-white">
                    <input type="text" placeholder="Name" class="px-3 py-3 w-full mb-5 border border-zinc-300 rounded">
                    <input type="email" placeholder="Email" class="px-3 py-3 w-full mb-5 border border-zinc-300 rounded">
                    <input type="text" placeholder="Query" class="px-3 py-3 w-full mb-5 border border-zinc-300 rounded">
                    <div class="mb-8">
                        <h3 class="mb-4 font-semibold text-sm text-zinc-800">Select Services</h3>
                        <div class="grid grid-cols-2 gap-4">
                            <div class="flex items-center" v-for="service in services" :key="service">
                                <input :id="service.id" type="checkbox" :value="service.name" class="w-4 h-4 text-blue-600 bg-gray-100 border-gray-300 rounded focus:ring-blue-500 dark:focus:ring-blue-600 dark:ring-offset-gray-800 focus:ring-2 dark:bg-gray-700 dark:border-gray-600">
                                <label :for="service.id" class="ml-2 text-sm font-medium text-zinc-600">{{ service.name }}</label>
                            </div>
                        </div>
                    </div>
                    <button class=" px-12 py-3 bg-zinc-800 text-white border rounded block">Submit</button>
                </div>
            </div>
            
        </div>
    </section>
</template>

<script setup>
    import { ref } from 'vue';

    const services = ref([
        {id: 1, name: 'SEO'},
        {id: 2, name: 'Content marketing'},
        {id: 3, name: 'Logo Design'},
        {id: 4, name: 'Web Design'},
        {id: 5, name: 'Illustration'},
        {id: 6, name: 'Influencer Marketing'}
    ])
</script>


<style scoped>
.contactSection{
    background-image: url("data:image/svg+xml,%3csvg xmlns='http://www.w3.org/2000/svg' version='1.1' xmlns:xlink='http://www.w3.org/1999/xlink' xmlns:svgjs='http://svgjs.com/svgjs' width='1440' height='560' preserveAspectRatio='none' viewBox='0 0 1440 560'%3e%3cg mask='url(%26quot%3b%23SvgjsMask1004%26quot%3b)' fill='none'%3e%3cpath d='M 0%2c199 C 57.6%2c167.8 172.8%2c36.2 288%2c43 C 403.2%2c49.8 460.8%2c241.6 576%2c233 C 691.2%2c224.4 748.8%2c4.2 864%2c0 C 979.2%2c-4.2 1036.8%2c205.4 1152%2c212 C 1267.2%2c218.6 1382.4%2c68.8 1440%2c33L1440 560L0 560z' fill='rgba(252%2c 252%2c 252%2c 1)'%3e%3c/path%3e%3cpath d='M 0%2c475 C 96%2c445.8 288%2c314 480%2c329 C 672%2c344 768%2c533 960%2c550 C 1152%2c567 1344%2c441.2 1440%2c414L1440 560L0 560z' fill='rgba(247%2c 247%2c 247%2c 1)'%3e%3c/path%3e%3c/g%3e%3cdefs%3e%3cmask id='SvgjsMask1004'%3e%3crect width='1440' height='560' fill='white'%3e%3c/rect%3e%3c/mask%3e%3c/defs%3e%3c/svg%3e");
    background-repeat: no-repeat;
    background-position: bottom;
}
</style>