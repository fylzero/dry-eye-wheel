<script setup>
import LottieAnimation from '@/lib/LottieAnimation.vue';
import EyelidsAnteriorBlepharitisExamJson from '@/assets/json/eyelids-anterior-blepharitis-exam.json';
</script>

<template>
    <LottieAnimation
        :json="EyelidsAnteriorBlepharitisExamJson"
        :loop="true"
        :autoPlay="true" />
</template>
