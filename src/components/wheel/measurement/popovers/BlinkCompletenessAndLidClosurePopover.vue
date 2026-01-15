<script setup>
import PopoverCard from '@/components/PopoverCard.vue';
import BlinkCompletenessAndLidClosureIcon from '@/components/wheel/measurement/animated-icons/BlinkCompletenessAndLidClosure.vue';
</script>

<template>
    <PopoverCard
        :title="$t('_blink_rate_and_completeness_title')"
        class="absolute left-1/2 top-[320px] z-10 col-span-5 ml-[-300px] max-w-lg">
        <template #icon>
            <BlinkCompletenessAndLidClosureIcon class="!-mb-8 !-mt-10 !h-40" />
        </template>
        {{ $t('_blink_rate_and_completeness_text') }}
    </PopoverCard>
</template>
