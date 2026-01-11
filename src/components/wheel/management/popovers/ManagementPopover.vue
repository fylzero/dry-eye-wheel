<script setup>
import PopoverCard from '@/components/PopoverCard.vue';
</script>

<template>
    <PopoverCard
        :title="$t('Management')"
        class="absolute left-1/2 top-[120px] z-10 col-span-5 ml-[-224px] max-w-md">
        <!-- TODO: Is display: contents supported widely enough? -->
        <span
            style="display: contents"
            v-html="$t('_management_text')" />
    </PopoverCard>
</template>
