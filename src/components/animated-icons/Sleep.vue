<script setup>
import LottieAnimation from '@/lib/LottieAnimation.vue';
import SleepJson from '@/assets/json/sleep.json';
</script>

<template>
    <LottieAnimation
        :json="SleepJson"
        :loop="true"
        :autoPlay="true" />
</template>
