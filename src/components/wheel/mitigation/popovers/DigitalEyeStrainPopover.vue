<script setup>
import Card from '@/components/Card.vue';
import DigitalEyeStrainIcon from '@/components/wheel/mitigation/animated-icons/DigitalEyeStrain.vue';
</script>

<template>
    <Card
        :title="$t('Digital Eye Strain')"
        class="absolute left-1/2 top-[240px] z-10 col-span-5 ml-[-224px] max-w-lg">
        <template #icon>
            <DigitalEyeStrainIcon class="!-mb-8 !-mt-10 !h-40" />
        </template>
        {{ $t('_digital_eye_strain_text') }}
    </Card>
</template>
