<script setup>
import LottieAnimation from '@/lib/LottieAnimation.vue';
import FluoresceinStainingJson from '@/assets/json/measurement/fluorescein-staining.json';
</script>

<template>
    <LottieAnimation
        :json="FluoresceinStainingJson"
        :loop="true"
        :autoPlay="true" />
</template>
