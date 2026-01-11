<script setup>
import LottieAnimation from '@/lib/LottieAnimation.vue';
import CornealSensitivityAssessmentJson from '@/assets/json/mitigation/corneal-sensitivity-assessment.json';
</script>

<template>
    <LottieAnimation
        :json="CornealSensitivityAssessmentJson"
        :loop="true"
        :autoPlay="true" />
</template>
