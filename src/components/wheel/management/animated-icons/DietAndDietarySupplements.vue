<script setup>
import LottieAnimation from '@/lib/LottieAnimation.vue';
import DietAndDietarySupplementsJson from '@/assets/json/management/diet-and-dietary-supplements.json';
</script>

<template>
    <LottieAnimation
        :json="DietAndDietarySupplementsJson"
        :loop="true"
        :autoPlay="true" />
</template>
