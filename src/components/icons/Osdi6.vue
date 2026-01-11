<script setup>
import LottieAnimation from '@/lib/LottieAnimation.vue';
import Osdi6Json from '@/assets/json/osdi-6.json';

const props = defineProps({
    targetId: {
        type: String,
        default: 'osdi6Animation',
    },
});
</script>

<template>
    <LottieAnimation
        :json="Osdi6Json"
        :loop="true"
        :autoPlay="true" />
</template>
