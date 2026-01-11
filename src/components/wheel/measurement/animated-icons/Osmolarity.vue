<script setup>
import LottieAnimation from '@/lib/LottieAnimation.vue';
import OsmolarityJson from '@/assets/json/measurement/osmolarity.json';
</script>

<template>
    <LottieAnimation
        :json="OsmolarityJson"
        :loop="true"
        :autoPlay="true" />
</template>
