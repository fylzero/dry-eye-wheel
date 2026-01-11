<script setup>
import LottieAnimation from '@/lib/LottieAnimation.vue';
import AqueousTearMeniscusHeightJson from '@/assets/json/aqueous-tear-meniscus-height.json';

const props = defineProps({
    targetId: {
        type: String,
        default: 'aqueousTearMeniscusHeightAnimation',
    },
});
</script>

<template>
    <LottieAnimation
        :json="AqueousTearMeniscusHeightJson"
        :loop="true"
        :autoPlay="true" />
</template>
