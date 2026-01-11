<script setup>
import LottieAnimation from '@/lib/LottieAnimation.vue';
import DigitalEyeStrainJson from '@/assets/json/digital-eye-strain.json';

const props = defineProps({
    targetId: {
        type: String,
        default: 'digitalEyeStrainAnimation',
    },
});
</script>

<template>
    <LottieAnimation
        :json="DigitalEyeStrainJson"
        :loop="true"
        :autoPlay="true" />
</template>
