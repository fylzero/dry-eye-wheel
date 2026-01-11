<script setup>
import LottieAnimation from '@/lib/LottieAnimation.vue';
import EyelidsAnteriorBlepharitisExamJson from '@/assets/json/eyelids-anterior-blepharitis-exam.json';

const props = defineProps({
    targetId: {
        type: String,
        default: 'eyelidsAnteriorBlepharitisExamAnimation',
    },
});
</script>

<template>
    <LottieAnimation
        :json="EyelidsAnteriorBlepharitisExamJson"
        :loop="true"
        :autoPlay="true" />
</template>
