<script setup>
import LottieAnimation from '@/lib/LottieAnimation.vue';
import HormonesJson from '@/assets/json/hormones.json';
</script>

<template>
    <LottieAnimation
        :json="HormonesJson"
        :loop="true"
        :autoPlay="true" />
</template>
