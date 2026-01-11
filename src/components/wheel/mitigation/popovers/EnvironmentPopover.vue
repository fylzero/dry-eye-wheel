<script setup>
import Card from '@/components/Card.vue';
import EnvironmentAdviceIcon from '@/components/animated-icons/Environment.vue';
</script>

<template>
    <Card
        :title="$t('Environment')"
        class="absolute left-1/2 top-[340px] z-10 col-span-5 ml-[-224px] max-w-lg">
        <template #icon>
            <EnvironmentAdviceIcon class="!-mb-8 !-mt-10 !h-40" />
        </template>

        {{ $t('_environment_text') }}
    </Card>
</template>
