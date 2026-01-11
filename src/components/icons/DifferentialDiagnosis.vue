<script setup>
import LottieAnimation from '@/lib/LottieAnimation.vue';
import DifferentialDiagnosisJson from '@/assets/json/differential-diagnosis.json';
</script>

<template>
    <LottieAnimation
        :json="DifferentialDiagnosisJson"
        :loop="true"
        :autoPlay="true" />
</template>
