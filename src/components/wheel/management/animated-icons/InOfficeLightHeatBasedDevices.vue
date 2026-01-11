<script setup>
import LottieAnimation from '@/lib/LottieAnimation.vue';
import InOfficeLightHeatBasedDevicesJson from '@/assets/json/management/in-office-light-heat-based-devices.json';
</script>

<template>
    <LottieAnimation
        :json="InOfficeLightHeatBasedDevicesJson"
        :loop="true"
        :autoPlay="true" />
</template>
