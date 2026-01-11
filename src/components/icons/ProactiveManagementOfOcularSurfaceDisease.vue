<script setup>
import LottieAnimation from '@/lib/LottieAnimation.vue';
import ProactiveManagementOfOcularSurfaceDiseaseJson from '@/assets/json/proactive-management-of-ocular-surface-disease.json';
</script>

<template>
    <LottieAnimation
        :json="ProactiveManagementOfOcularSurfaceDiseaseJson"
        :loop="true"
        :autoPlay="true" />
</template>
