<script setup>
import LottieAnimation from '@/lib/LottieAnimation.vue';
import BlinkCompletenessAndLidClosureJson from '@/assets/json/blink-rate-completeness.json';

const props = defineProps({
    targetId: {
        type: String,
        default: 'BlinkCompletenessAndLidClosureAnimation',
    },
});
</script>

<template>
    <LottieAnimation
        :json="BlinkCompletenessAndLidClosureJson"
        :loop="true"
        :autoPlay="true" />
</template>
