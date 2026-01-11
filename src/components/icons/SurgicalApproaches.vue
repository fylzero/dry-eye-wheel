<script setup>
import LottieAnimation from '@/lib/LottieAnimation.vue';
import SurgicalApproachesJson from '@/assets/json/surgical-approaches.json';

const props = defineProps({
    targetId: {
        type: String,
        default: 'surgicalApproachesAnimation',
    },
});
</script>

<template>
    <LottieAnimation
        :json="SurgicalApproachesJson"
        :loop="true"
        :autoPlay="true" />
</template>
