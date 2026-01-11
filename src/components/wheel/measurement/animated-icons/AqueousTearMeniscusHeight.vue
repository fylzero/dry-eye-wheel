<script setup>
import LottieAnimation from '@/lib/LottieAnimation.vue';
import AqueousTearMeniscusHeightJson from '@/assets/json/measurement/aqueous-tear-meniscus-height.json';
</script>

<template>
    <LottieAnimation
        :json="AqueousTearMeniscusHeightJson"
        :loop="true"
        :autoPlay="true" />
</template>
