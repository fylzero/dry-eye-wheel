<script setup>
import LottieAnimation from '@/lib/LottieAnimation.vue';
import EnvironmentJson from '@/assets/json/environment.json';
</script>

<template>
    <LottieAnimation
        :json="EnvironmentJson"
        :loop="true"
        :autoPlay="true" />
</template>
