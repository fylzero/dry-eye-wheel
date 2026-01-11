<script setup>
import PopoverCard from '@/components/PopoverCard.vue';
import PharmaceuticalsIcon from '@/components/wheel/management/animated-icons/Pharmaceuticals.vue';
</script>

<template>
    <PopoverCard
        :title="$t('Pharmaceuticals')"
        class="absolute left-1/2 top-[240px] z-10 col-span-5 ml-[-224px] max-w-xl">
        <template #icon>
            <PharmaceuticalsIcon class="!-mb-6 !h-40" />
        </template>
        {{ $t('_pharmaceuticals_text') }}
    </PopoverCard>
</template>
