<script setup>
import { useControlsStore } from '@/stores/controlsStore.js';
const controlsStore = useControlsStore();
</script>

<template>
    <g
        class="svg-icon"
        :class="{ 'svg-active': controlsStore.selectedItem === 'eyelids-anterior-blepharitis-exam' }"
        style="transform: translate(420px, 96px)">
        <!-- Icon -->
        <g>
            <circle
                cx="200"
                cy="320"
                r="15"
                fill="black" />
        </g>

        <!-- Use _eyelids_anterior_blepharitis_exam_title translation with | as line break delimiter -->
        <text
            x="200"
            y="346"
            text-anchor="middle">
            <tspan
                v-for="(line, index) in $t('_eyelids_anterior_blepharitis_exam_title').split('|')"
                :key="index"
                x="200"
                :dy="index === 0 ? 0 : 12"
                :style="$selectedLanguage.value === 'zh' ? 'font-size: 14px !important;' : ''">
                {{ line }}
            </tspan>
        </text>
    </g>
</template>
