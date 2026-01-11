<script setup>
import LottieAnimation from '@/lib/LottieAnimation.vue';
import SurgicalApproachesJson from '@/assets/json/surgical-approaches.json';
</script>

<template>
    <LottieAnimation
        :json="SurgicalApproachesJson"
        :loop="true"
        :autoPlay="true" />
</template>
