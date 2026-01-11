<script setup>
import LottieAnimation from '@/lib/LottieAnimation.vue';
import SymptomCheckJson from '@/assets/json/mitigation/symptom-check.json';
</script>

<template>
    <LottieAnimation
        :json="SymptomCheckJson"
        :loop="true"
        :autoPlay="true" />
</template>
