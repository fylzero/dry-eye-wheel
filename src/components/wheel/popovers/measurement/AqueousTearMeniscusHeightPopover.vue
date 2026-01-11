<script setup>
import Card from '@/components/Card.vue';
import AqueousTearMeniscusHeightIcon from '@/components/icons/AqueousTearMeniscusHeight.vue';
</script>

<template>
    <Card
        :title="$t('Aqueous Tear Meniscus Height')"
        class="absolute left-1/2 top-[340px] z-10 col-span-5 ml-[-340px] max-w-lg">
        <template #icon>
            <AqueousTearMeniscusHeightIcon class="!-mb-8 !-mt-10 !h-40" />
        </template>
        <div
            class="contents"
            v-html="$t('_aqueous_tear_meniscus_height_text')" />
    </Card>
</template>
