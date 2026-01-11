<script setup>
import LottieAnimation from '@/lib/LottieAnimation.vue';
import ContactLensJson from '@/assets/json/contact-lens.json';
</script>

<template>
    <LottieAnimation
        :json="ContactLensJson"
        :loop="true"
        :autoPlay="true" />
</template>
