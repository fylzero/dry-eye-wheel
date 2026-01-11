<script setup>
import LottieAnimation from '@/lib/LottieAnimation.vue';
import LidHygieneJson from '@/assets/json/management/lid-hygiene.json';
</script>

<template>
    <LottieAnimation
        :json="LidHygieneJson"
        :loop="true"
        :autoPlay="true" />
</template>
