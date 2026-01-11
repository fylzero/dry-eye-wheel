<script setup>
import { useControlsStore } from '@/stores/controlsStore.js';
const controlsStore = useControlsStore();
</script>

<template>
    <g
        class="svg-icon"
        :class="{ 'svg-active': controlsStore.selectedItem === 'corneal-sensitivity-assessment' }"
        style="transform: translate(0px, 40px)">
        <!-- Icon -->
        <g>
            <circle
                cx="200"
                cy="320"
                r="15"
                fill="black" />
        </g>

        <text
            x="200"
            y="340"
            text-anchor="middle"
            :style="$selectedLanguage.value === 'zh' ? 'font-size: 14px !important;' : ''">
            {{ $t('Corneal Sensitivity Assessment') }}
        </text>
    </g>
</template>
