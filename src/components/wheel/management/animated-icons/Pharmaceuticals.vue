<script setup>
import LottieAnimation from '@/lib/LottieAnimation.vue';
import PharmaceuticalsJson from '@/assets/json/management/pharmaceuticals.json';
</script>

<template>
    <LottieAnimation
        :json="PharmaceuticalsJson"
        :loop="true"
        :autoPlay="true" />
</template>
