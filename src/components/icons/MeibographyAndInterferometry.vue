<script setup>
import LottieAnimation from '@/lib/LottieAnimation.vue';
import MeibographyAndInterferometryJson from '@/assets/json/meibography-and-interferometry.json';

const props = defineProps({
    targetId: {
        type: String,
        default: 'meibographyAndInterferometryAnimation',
    },
});
</script>

<template>
    <LottieAnimation
        :json="MeibographyAndInterferometryJson"
        :loop="true"
        :autoPlay="true" />
</template>
