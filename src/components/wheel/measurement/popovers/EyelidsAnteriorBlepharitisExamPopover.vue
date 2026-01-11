<script setup>
import Card from '@/components/Card.vue';
import EyelidsAnteriorBlepharitisExamIcon from '@/components/wheel/measurement/animated-icons/EyelidsAnteriorBlepharitisExam.vue';
</script>

<template>
    <Card
        :title="$t('Eyelids: Anterior Blepharitis Exam')"
        class="absolute left-1/2 top-[240px] z-10 col-span-5 ml-[-224px] max-w-lg">
        <template #icon>
            <EyelidsAnteriorBlepharitisExamIcon class="!-mb-8 !-mt-10 !h-40" />
        </template>
        {{ $t('_eyelids_anterior_blepharitis_exam_text') }}
    </Card>
</template>
