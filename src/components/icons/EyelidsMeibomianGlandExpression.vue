<script setup>
import LottieAnimation from '@/lib/LottieAnimation.vue';
import EyelidsMeibomianGlandExpressionJson from '@/assets/json/eyelids-meibomian-gland-expression.json';

const props = defineProps({
    targetId: {
        type: String,
        default: 'eyelidsMeibomianGlandExpressionAnimation',
    },
});
</script>

<template>
    <LottieAnimation
        :json="EyelidsMeibomianGlandExpressionJson"
        :loop="true"
        :autoPlay="true" />
</template>
