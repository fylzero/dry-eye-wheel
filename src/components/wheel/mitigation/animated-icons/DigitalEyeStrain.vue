<script setup>
import LottieAnimation from '@/lib/LottieAnimation.vue';
import DigitalEyeStrainJson from '@/assets/json/mitigation/digital-eye-strain.json';
</script>

<template>
    <LottieAnimation
        :json="DigitalEyeStrainJson"
        :loop="true"
        :autoPlay="true" />
</template>
