<script setup>
import LottieAnimation from '@/lib/LottieAnimation.vue';
import LissamineGreenStaningJson from '@/assets/json/lissamine-green-staning.json';
</script>

<template>
    <LottieAnimation
        :json="LissamineGreenStaningJson"
        :loop="true"
        :autoPlay="true" />
</template>
