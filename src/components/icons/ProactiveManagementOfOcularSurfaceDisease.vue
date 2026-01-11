<script setup>
import LottieAnimation from '@/lib/LottieAnimation.vue';
import ProactiveManagementOfOcularSurfaceDiseaseJson from '@/assets/json/proactive-management-of-ocular-surface-disease.json';

const props = defineProps({
    targetId: {
        type: String,
        default: 'proactiveManagementOfOcularSurfaceDiseaseAnimation',
    },
});
</script>

<template>
    <LottieAnimation
        :json="ProactiveManagementOfOcularSurfaceDiseaseJson"
        :loop="true"
        :autoPlay="true" />
</template>
