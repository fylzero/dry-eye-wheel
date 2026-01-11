<script setup>
import { useControlsStore } from '@/stores/controlsStore.js';
const controlsStore = useControlsStore();
</script>

<template>
    <g
        class="svg-icon"
        :class="{ 'svg-active': controlsStore.selectedItem === 'corneal-sensitivity-assessment' }"
        style="transform: translate(130px, -60px)">
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
            y="346"
            text-anchor="middle">
            <tspan
                v-for="(line, index) in $t('_corneal_sensitivity_assessment_icon').split('|')"
                :key="index"
                x="200"
                :dy="index === 0 ? 0 : 12"
                :style="$selectedLanguage.value === 'zh' ? 'font-size: 14px !important;' : ''">
                {{ line }}
            </tspan>
        </text>
    </g>
</template>
