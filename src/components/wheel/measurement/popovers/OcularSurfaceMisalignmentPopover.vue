<script setup>
import Card from '@/components/Card.vue';
import OcularSurfaceMisalignmentIcon from '@/components/wheel/measurement/animated-icons/OcularSurfaceMisalignment.vue';
</script>

<template>
    <Card
        :title="$t('Ocular Surface Misalignment')"
        class="absolute left-1/2 top-[240px] z-10 col-span-5 ml-[-224px] max-w-lg">
        <template #icon>
            <OcularSurfaceMisalignmentIcon class="!-mb-8 !-mt-10 !h-40" />
        </template>
        {{ $t('_ocular_surface_misalignment_text') }}
    </Card>
</template>
