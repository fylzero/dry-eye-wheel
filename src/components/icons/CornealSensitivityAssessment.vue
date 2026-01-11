<script setup>
import LottieAnimation from '@/lib/LottieAnimation.vue';
import CornealSensitivityAssessmentJson from '@/assets/json/corneal-sensitivity-assessment.json';

const props = defineProps({
    targetId: {
        type: String,
        default: 'cornealSensitivityAssessmentAnimation',
    },
});
</script>

<template>
    <LottieAnimation
        :json="CornealSensitivityAssessmentJson"
        :loop="true"
        :autoPlay="true" />
</template>
