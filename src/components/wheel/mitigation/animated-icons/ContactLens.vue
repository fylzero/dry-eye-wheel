<script setup>
import LottieAnimation from '@/lib/LottieAnimation.vue';
import ContactLensJson from '@/assets/json/mitigation/contact-lens.json';
</script>

<template>
    <LottieAnimation
        :json="ContactLensJson"
        :loop="true"
        :autoPlay="true" />
</template>
