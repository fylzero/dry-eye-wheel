<script setup>
import LottieAnimation from '@/lib/LottieAnimation.vue';
import ProphylaxisJson from '@/assets/json/mitigation/prophylaxis.json';
</script>

<template>
    <LottieAnimation
        :json="ProphylaxisJson"
        :loop="true"
        :autoPlay="true" />
</template>
