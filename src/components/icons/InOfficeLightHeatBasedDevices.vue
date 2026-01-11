<script setup>
import LottieAnimation from '@/lib/LottieAnimation.vue';
import InOfficeLightHeatBasedDevicesJson from '@/assets/json/in-office-light-heat-based-devices.json';

const props = defineProps({
    targetId: {
        type: String,
        default: 'inOfficeLightHeatBasedDevicesAnimation',
    },
});
</script>

<template>
    <LottieAnimation
        :json="InOfficeLightHeatBasedDevicesJson"
        :loop="true"
        :autoPlay="true" />
</template>
