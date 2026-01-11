<script setup>
import LottieAnimation from '@/lib/LottieAnimation.vue';
import DietAndDietarySupplementsJson from '@/assets/json/diet-and-dietary-supplements.json';
</script>

<template>
    <LottieAnimation
        :json="DietAndDietarySupplementsJson"
        :loop="true"
        :autoPlay="true" />
</template>
