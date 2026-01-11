<script setup>
import LottieAnimation from '@/lib/LottieAnimation.vue';
import BlinkExercisesJson from '@/assets/json/management/blink-exercises.json';
</script>

<template>
    <LottieAnimation
        :json="BlinkExercisesJson"
        :loop="true"
        :autoPlay="true" />
</template>
