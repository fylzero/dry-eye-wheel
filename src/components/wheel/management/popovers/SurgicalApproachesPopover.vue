<script setup>
import Card from '@/components/Card.vue';
import SurgicalApproachesIcon from '@/components/animated-icons/SurgicalApproaches.vue';
</script>

<template>
    <Card
        :title="$t('Surgical Approaches')"
        class="absolute left-1/2 top-[180px] z-10 col-span-5 ml-[-260px] max-w-xl">
        <template #icon>
            <SurgicalApproachesIcon class="!-mb-8 !-mt-10 !h-40" />
        </template>

        {{ $t('_surgical_approaches_text') }}
    </Card>
</template>
