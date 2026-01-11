<script setup>
import LottieAnimation from '@/lib/LottieAnimation.vue';
import ComplexTreatmentsJson from '@/assets/json/complex-treatments.json';
</script>

<template>
    <LottieAnimation
        :json="ComplexTreatmentsJson"
        :loop="true"
        :autoPlay="true" />
</template>
