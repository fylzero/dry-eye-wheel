<script setup>
import PopoverCard from '@/components/PopoverCard.vue';
</script>

<template>
    <PopoverCard
        :title="$t('Mitigation')"
        class="absolute left-1/2 top-[360px] z-10 col-span-5 ml-[-80px] max-w-md">
        <div
            class="contents"
            v-html="$t('_mitigation_text')" />
    </PopoverCard>
</template>
