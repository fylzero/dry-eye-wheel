<script setup>
import LottieAnimation from '@/lib/LottieAnimation.vue';
import SymptomCheckJson from '@/assets/json/symptom-check.json';
</script>

<template>
    <LottieAnimation
        :json="SymptomCheckJson"
        :loop="true"
        :autoPlay="true" />
</template>
