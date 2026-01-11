<script setup>
import Card from '@/components/Card.vue';
import Osdi6Icon from '@/components/wheel/measurement/animated-icons/Osdi6.vue';
</script>

<template>
    <Card
        :title="$t('OSDI-6')"
        class="absolute left-1/2 top-[220px] z-10 col-span-5 ml-[-240px] max-w-lg">
        <template #icon>
            <Osdi6Icon class="!-mb-8 !-mt-10 !h-40" />
        </template>

        <div
            class="contents"
            v-html="$t('_osdi_6_text')" />
    </Card>
</template>
