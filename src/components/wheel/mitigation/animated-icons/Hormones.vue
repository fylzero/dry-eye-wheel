<script setup>
import LottieAnimation from '@/lib/LottieAnimation.vue';
import HormonesJson from '@/assets/json/mitigation/hormones.json';
</script>

<template>
    <LottieAnimation
        :json="HormonesJson"
        :loop="true"
        :autoPlay="true" />
</template>
