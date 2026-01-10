<script setup>
import { useControlsStore } from '@/stores/controlsStore.js';
const controlsStore = useControlsStore();
</script>

<template>
    <g
        class="svg-icon"
        :class="{ 'svg-active': controlsStore.selectedItem === 'hormones' }"
        style="transform: translate(0px, 0px)">
        <!-- Icon -->
        <g>
            <g>
                <polygon
                    class="mitigation-cls-10"
                    points="266.51 409.24 277.78 423.94 255.23 423.94 266.51 409.24" />
                <circle
                    class="mitigation-cls-5"
                    cx="248.35"
                    cy="405.78"
                    r="6.16" />
                <rect
                    x="240.92"
                    y="406.61"
                    width="49.51"
                    height="3.87"
                    rx="1.31"
                    ry="1.31"
                    transform="translate(-119.8 110.38) rotate(-19.24)" />
                <circle
                    class="mitigation-cls-5"
                    cx="277.05"
                    cy="396.07"
                    r="6.16" />
                <g>
                    <line
                        class="mitigation-cls-14"
                        x1="251.71"
                        y1="400.33"
                        x2="256.44"
                        y2="392.53" />
                    <g>
                        <line
                            class="mitigation-cls-9"
                            x1="251.71"
                            y1="400.33"
                            x2="254.58"
                            y2="395.6" />
                        <polygon points="256.33 397.52 256.44 392.53 252.07 394.93 256.33 397.52" />
                    </g>
                </g>
            </g>
            <line
                class="mitigation-cls-8"
                x1="272.78"
                y1="391.5"
                x2="268.27"
                y2="384.93" />
            <line
                class="mitigation-cls-7"
                x1="272.27"
                y1="385.77"
                x2="267.49"
                y2="389.02" />
        </g>
        <text
            x="266"
            y="440"
            text-anchor="middle">
            {{ $t('Hormones') }}
        </text>
    </g>
</template>
<style scoped lang="postcss">
.cls-1,
.cls-2 {
    fill: none;
}

.cls-1,
.cls-2,
.cls-3,
.cls-4,
.cls-5 {
    stroke: #000;
}

.cls-1,
.cls-2,
.cls-4,
.cls-5 {
    stroke-width: 2px;
}

.cls-1,
.cls-4,
.cls-5 {
    stroke-miterlimit: 10;
}

.cls-2,
.cls-3 {
    stroke-linejoin: round;
}

.cls-2,
.cls-3,
.cls-4,
.cls-5 {
    stroke-linecap: round;
}

.cls-4 {
    fill: url(#linear-gradient-2);
}

.cls-5 {
    fill: url(#linear-gradient-3);
}

.cls-6 {
    fill: url(#linear-gradient);
}
</style>
