<script setup>
import PopoverCard from '@/components/PopoverCard.vue';
import ProactiveManagementOfOcularSurfaceDiseaseIcon from '@/components/wheel/mitigation/animated-icons/ProactiveManagementOfOcularSurfaceDisease.vue';
</script>

<template>
    <PopoverCard
        :title="$t('_proactive_management_of_ocular_surface_disease_title')"
        class="absolute left-1/2 top-[240px] z-10 col-span-5 ml-[-224px] max-w-lg">
        <template #icon>
            <ProactiveManagementOfOcularSurfaceDiseaseIcon class="!-mb-8 !-mt-10 !h-40" />
        </template>
        {{ $t('_proactive_management_of_ocular_surface_disease_text') }}
    </PopoverCard>
</template>
