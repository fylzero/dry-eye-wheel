<script setup>
import LottieAnimation from '@/lib/LottieAnimation.vue';
import OcularSurfaceMisalignmentJson from '@/assets/json/ocular-surface-misalignment.json';

const props = defineProps({
    targetId: {
        type: String,
        default: 'ocularSurfaceMisalignmentAnimation',
    },
});
</script>

<template>
    <LottieAnimation
        :json="OcularSurfaceMisalignmentJson"
        :loop="true"
        :autoPlay="true" />
</template>
