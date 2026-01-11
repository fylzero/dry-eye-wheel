<script setup>
import LottieAnimation from '@/lib/LottieAnimation.vue';
import Osdi6Json from '@/assets/json/osdi-6.json';
</script>

<template>
    <LottieAnimation
        :json="Osdi6Json"
        :loop="true"
        :autoPlay="true" />
</template>
