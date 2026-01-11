<script setup>
import Card from '@/components/Card.vue';
import MeibographyAndInterferometryIcon from '@/components/wheel/measurement/animated-icons/MeibographyAndInterferometry.vue';
</script>

<template>
    <Card
        :title="$t('Meibography and Interferometry')"
        class="absolute left-1/2 top-[380px] z-10 col-span-5 ml-[-300px] max-w-xl">
        <template #icon>
            <MeibographyAndInterferometryIcon class="!-mb-8 !-mt-10 !h-40" />
        </template>
        {{ $t('_meibography_and_interferometry_text') }}
    </Card>
</template>
