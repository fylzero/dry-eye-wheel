<script setup>
import LottieAnimation from '@/lib/LottieAnimation.vue';
import AdviceJson from '@/assets/json/advice.json';
</script>

<template>
    <LottieAnimation
        :json="AdviceJson"
        :loop="true"
        :autoPlay="true" />
</template>
