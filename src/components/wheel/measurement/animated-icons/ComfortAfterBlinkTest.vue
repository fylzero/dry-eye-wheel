<script setup>
import LottieAnimation from '@/lib/LottieAnimation.vue';
import ComfortAfterBlinkTestJson from '@/assets/json/measurement/comfort-after-blink-test.json';
</script>

<template>
    <LottieAnimation
        :json="ComfortAfterBlinkTestJson"
        :loop="true"
        :autoPlay="true" />
</template>
