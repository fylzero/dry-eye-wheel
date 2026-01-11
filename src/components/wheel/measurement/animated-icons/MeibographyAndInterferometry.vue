<script setup>
import LottieAnimation from '@/lib/LottieAnimation.vue';
import MeibographyAndInterferometryJson from '@/assets/json/measurement/meibography-and-interferometry.json';
</script>

<template>
    <LottieAnimation
        :json="MeibographyAndInterferometryJson"
        :loop="true"
        :autoPlay="true" />
</template>
