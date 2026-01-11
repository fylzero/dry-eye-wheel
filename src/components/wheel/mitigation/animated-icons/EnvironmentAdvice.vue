<script setup>
import LottieAnimation from '@/lib/LottieAnimation.vue';
import EnvironmentJson from '@/assets/json/mitigation/environment-advice.json';
</script>

<template>
    <LottieAnimation
        :json="EnvironmentJson"
        :loop="true"
        :autoPlay="true" />
</template>
