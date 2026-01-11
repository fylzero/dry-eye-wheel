<script setup>
import LottieAnimation from '@/lib/LottieAnimation.vue';
import DigitalEyeStrainJson from '@/assets/json/digital-eye-strain.json';
</script>

<template>
    <LottieAnimation
        :json="DigitalEyeStrainJson"
        :loop="true"
        :autoPlay="true" />
</template>
