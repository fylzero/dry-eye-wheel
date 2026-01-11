<script setup>
import Card from '@/components/Card.vue';
import ProactiveManagementOfOcularSurfaceDiseaseIcon from '@/components/icons/ProactiveManagementOfOcularSurfaceDisease.vue';
</script>

<template>
    <Card
        :title="$t('Proactive Management of Ocular Surface Disease')"
        class="absolute left-1/2 top-[240px] z-10 col-span-5 ml-[-224px] max-w-lg">
        <template #icon>
            <ProactiveManagementOfOcularSurfaceDiseaseIcon class="!-mb-8 !-mt-10 !h-40" />
        </template>
        {{ $t('_proactive_management_of_ocular_surface_disease_text') }}
    </Card>
</template>
