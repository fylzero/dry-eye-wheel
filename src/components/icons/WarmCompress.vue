<script setup>
import LottieAnimation from '@/lib/LottieAnimation.vue';
import WarmCompressJson from '@/assets/json/warm-compress.json';
</script>

<template>
    <LottieAnimation
        :json="WarmCompressJson"
        :loop="true"
        :autoPlay="true" />
</template>
