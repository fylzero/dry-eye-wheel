<script setup>
import { useControlsStore } from '@/stores/controlsStore.js';
import MeasurementPopover from '@/components/wheel/measurement/popovers/MeasurementPopover.vue';
import ComfortAfterBlinkTestPopover from '@/components/wheel/measurement/popovers/ComfortAfterBlinkTestPopover.vue';
import Osdi6Popover from '@/components/wheel/measurement/popovers/Osdi6Popover.vue';
import FluoresceinStainingPopover from '@/components/wheel/measurement/popovers/FluoresceinStainingPopover.vue';
import NonInvasiveBreakupTimePopover from '@/components/wheel/measurement/popovers/NonInvasiveBreakupTimePopover.vue';
import OsmolarityPopover from '@/components/wheel/measurement/popovers/OsmolarityPopover.vue';
import LissamineGreenStainingPopover from '@/components/wheel/measurement/popovers/LissamineGreenStainingPopover.vue';
import BlinkCompletenessAndLidClosurePopover from '@/components/wheel/measurement/popovers/BlinkCompletenessAndLidClosurePopover.vue';
import AqueousTearMeniscusHeightPopover from '@/components/wheel/measurement/popovers/AqueousTearMeniscusHeightPopover.vue';
import EyelidsMeibomianGlandExpressionPopover from '@/components/wheel/measurement/popovers/EyelidsMeibomianGlandExpressionPopover.vue';
import MeibographyAndInterferometryPopover from '@/components/wheel/measurement/popovers/MeibographyAndInterferometryPopover.vue';
import OcularSurfaceMisalignmentPopover from '@/components/wheel/measurement/popovers/OcularSurfaceMisalignmentPopover.vue';
import EyelidsAnteriorBlepharitisExamPopover from '@/components/wheel/measurement/popovers/EyelidsAnteriorBlepharitisExamPopover.vue';

const controlsStore = useControlsStore();
</script>

<template>
    <MeasurementPopover
        v-if="
            controlsStore.selectedArea === 'measurement' &&
            !controlsStore.selectedSection &&
            !controlsStore.selectedItem
        " />

    <!-- Section Popovers -->
    <ComfortAfterBlinkTestPopover v-if="controlsStore.selectedItem === 'comfort-time-after-blink-test'" />
    <Osdi6Popover v-if="controlsStore.selectedItem === 'osdi-6'" />
    <FluoresceinStainingPopover v-if="controlsStore.selectedItem === 'fluorescein-staining'" />
    <NonInvasiveBreakupTimePopover v-if="controlsStore.selectedItem === 'non-invasive-breakup-time'" />
    <OsmolarityPopover v-if="controlsStore.selectedItem === 'osmolarity'" />
    <LissamineGreenStainingPopover v-if="controlsStore.selectedItem === 'lissamine-green-staining'" />
    <BlinkCompletenessAndLidClosurePopover v-if="controlsStore.selectedItem === 'blink-rate-and-completeness'" />
    <AqueousTearMeniscusHeightPopover v-if="controlsStore.selectedItem === 'aqueous-tear-meniscus-height'" />
    <EyelidsMeibomianGlandExpressionPopover
        v-if="controlsStore.selectedItem === 'eyelids-meibomian-gland-expression'" />
    <MeibographyAndInterferometryPopover v-if="controlsStore.selectedItem === 'meibography-and-interferometry'" />
    <OcularSurfaceMisalignmentPopover v-if="controlsStore.selectedItem === 'ocular-surface-misalignment'" />
    <EyelidsAnteriorBlepharitisExamPopover v-if="controlsStore.selectedItem === 'eyelids-anterior-blepharitis-exam'" />
</template>
