<script setup>
import LottieAnimation from '@/lib/LottieAnimation.vue';
import BlinkCompletenessAndLidClosureJson from '@/assets/json/measurement/blink-rate-completeness.json';
</script>

<template>
    <LottieAnimation
        :json="BlinkCompletenessAndLidClosureJson"
        :loop="true"
        :autoPlay="true" />
</template>
