<script setup>
import Card from '@/components/Card.vue';
import AdviceIcon from '@/components/icons/Advice.vue';
</script>

<template>
    <Card
        :title="$t('Symptom Check')"
        class="absolute left-1/2 top-[220px] z-10 col-span-5 ml-[-224px] max-w-md">
        <template #icon>
            <AdviceIcon class="!-mb-8 !-mt-10 !h-40" />
        </template>
        {{ $t('_symptom_check_text') }}
    </Card>
</template>
