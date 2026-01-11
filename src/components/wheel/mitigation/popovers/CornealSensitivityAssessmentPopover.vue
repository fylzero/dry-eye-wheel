<script setup>
import Card from '@/components/Card.vue';
import CornealSensitivityAssessmentIcon from '@/components/wheel/mitigation/animated-icons/CornealSensitivityAssessment.vue';
</script>

<template>
    <Card
        :title="$t('Corneal Sensitivity Assessment')"
        class="absolute left-1/2 top-[240px] z-10 col-span-5 ml-[-224px] max-w-lg">
        <template #icon>
            <CornealSensitivityAssessmentIcon class="!-mb-8 !-mt-10 !h-40" />
        </template>
        {{ $t('_corneal_sensitivity_assessment_text') }}
    </Card>
</template>
