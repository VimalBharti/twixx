<template>
    <div class="bg-white">
        <Slides />
        <Service id="service" />
        <Work id="work" />
        <Contact id="contact" />
    </div>
</template>

<script setup>
    import { ref } from 'vue';
    import Slides from '../views/Slides.vue'
    import Service from '../views/Service.vue'
    import Work from '../views/Work.vue'
    import Contact from '../views/Contact.vue'

</script>