<script setup>
import LottieAnimation from '@/lib/LottieAnimation.vue';
import EyelidsMeibomianGlandExpressionJson from '@/assets/json/eyelids-meibomian-gland-expression.json';
</script>

<template>
    <LottieAnimation
        :json="EyelidsMeibomianGlandExpressionJson"
        :loop="true"
        :autoPlay="true" />
</template>
