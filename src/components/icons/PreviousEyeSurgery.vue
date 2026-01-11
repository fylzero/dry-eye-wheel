<script setup>
import LottieAnimation from '@/lib/LottieAnimation.vue';
import PreviousEyeSurgeryJson from '@/assets/json/previous-eye-surgery.json';
</script>

<template>
    <LottieAnimation
        :json="PreviousEyeSurgeryJson"
        :loop="true"
        :autoPlay="true" />
</template>
