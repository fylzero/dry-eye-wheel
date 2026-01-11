<script setup>
import { useControlsStore } from '@/stores/controlsStore.js';
import ManagementPopover from '@/components/wheel/management/popovers/ManagementPopover.vue';
import LidHygienePopover from '@/components/wheel/management/popovers/LidHygienePopover.vue';
import WarmCompressPopover from '@/components/wheel/management/popovers/WarmCompressPopover.vue';
import BlinkExercisesPopover from '@/components/wheel/management/popovers/BlinkExercisesPopover.vue';
import AdvicePopover from '@/components/wheel/management/popovers/AdvicePopover.vue';
import ArtificialTearsPopover from '@/components/wheel/management/popovers/ArtificialTearsPopover.vue';
import InOfficeLightHeatBasedDevicesPopover from '@/components/wheel/management/popovers/InOfficeLightHeatBasedDevicesPopover.vue';
import DietAndDietarySupplementsPopover from '@/components/wheel/management/popovers/DietAndDietarySupplementsPopover.vue';
import PharmaceuticalsPopover from '@/components/wheel/management/popovers/PharmaceuticalsPopover.vue';
import ScleralLensesPopover from '@/components/wheel/management/popovers/ScleralLensesPopover.vue';
import SurgicalApproachesPopover from '@/components/wheel/management/popovers/SurgicalApproachesPopover.vue';
import ComplexTreatmentsPopover from '@/components/wheel/management/popovers/ComplexTreatmentsPopover.vue';

const controlsStore = useControlsStore();
</script>

<template>
    <ManagementPopover
        v-if="
            controlsStore.selectedArea === 'management' && !controlsStore.selectedSection && !controlsStore.selectedItem
        " />

    <!-- Management Section Popovers -->
    <LidHygienePopover v-if="controlsStore.selectedItem === 'lid-hygiene'" />
    <WarmCompressPopover v-if="controlsStore.selectedItem === 'warm-compress'" />
    <BlinkExercisesPopover v-if="controlsStore.selectedItem === 'blink-exercises'" />
    <AdvicePopover v-if="controlsStore.selectedItem === 'advice'" />
    <DietAndDietarySupplementsPopover v-if="controlsStore.selectedItem === 'diet-and-dietary-supplements'" />
    <ArtificialTearsPopover v-if="controlsStore.selectedItem === 'artificial-tears'" />
    <InOfficeLightHeatBasedDevicesPopover v-if="controlsStore.selectedItem === 'in-office-light-heat-based-devices'" />
    <PharmaceuticalsPopover v-if="controlsStore.selectedItem === 'pharmaceuticals'" />
    <ScleralLensesPopover v-if="controlsStore.selectedItem === 'scleral-lenses'" />
    <SurgicalApproachesPopover v-if="controlsStore.selectedItem === 'surgical-approaches'" />
    <ComplexTreatmentsPopover v-if="controlsStore.selectedItem === 'complex-treatments'" />
</template>
