<script setup>
import LottieAnimation from '@/lib/LottieAnimation.vue';
import ScleralLensesJson from '@/assets/json/management/scleral-lenses.json';
</script>

<template>
    <LottieAnimation
        :json="ScleralLensesJson"
        :loop="true"
        :autoPlay="true" />
</template>
