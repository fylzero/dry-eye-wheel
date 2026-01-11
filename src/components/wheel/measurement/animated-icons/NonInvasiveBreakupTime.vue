<script setup>
import LottieAnimation from '@/lib/LottieAnimation.vue';
import BreakupTimeJson from '@/assets/json/measurement/non-invasive-breakup-time.json';
</script>

<template>
    <LottieAnimation
        :json="BreakupTimeJson"
        :loop="true"
        :autoPlay="true" />
</template>
