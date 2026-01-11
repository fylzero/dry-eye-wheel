<script setup>
import Card from '@/components/Card.vue';
import PreviousEyeSurgeryIcon from '@/components/wheel/mitigation/animated-icons/PreviousEyeSurgery.vue';
</script>

<template>
    <Card
        :title="$t('Previous Eye Surgery')"
        class="absolute left-1/2 top-[240px] z-10 col-span-5 ml-[-224px] max-w-lg">
        <template #icon>
            <PreviousEyeSurgeryIcon class="!-mb-8 !-mt-10 !h-40" />
        </template>
        {{ $t('_previous_eye_surgery_text') }}
    </Card>
</template>
