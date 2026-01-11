<script setup>
import LottieAnimation from '@/lib/LottieAnimation.vue';
import OcularSurfaceMisalignmentJson from '@/assets/json/measurement/ocular-surface-misalignment.json';
</script>

<template>
    <LottieAnimation
        :json="OcularSurfaceMisalignmentJson"
        :loop="true"
        :autoPlay="true" />
</template>
