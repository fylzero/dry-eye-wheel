<script setup>
import { useControlsStore } from '@/stores/controlsStore.js';
import MitigationPopover from '@/components/wheel/popovers/MitigationPopover.vue';
import QuestionnaireForEarlyIdPopover from '@/components/wheel/popovers/mitigation/QuestionnaireForEarlyIdPopover.vue';
import DifferentialDiagnosisPopover from '@/components/wheel/popovers/mitigation/DifferentialDiagnosisPopover.vue';
import ProphylaxisPopover from '@/components/wheel/popovers/mitigation/ProphylaxisPopover.vue';
import SleepPopover from '@/components/wheel/popovers/mitigation/SleepPopover.vue';
import ContactLensesPopover from '@/components/wheel/popovers/mitigation/ContactLensesPopover.vue';
import DigitalEyeStrainPopover from '@/components/wheel/popovers/mitigation/DigitalEyeStrainPopover.vue';
import EnvironmentPopover from '@/components/wheel/popovers/mitigation/EnvironmentPopover.vue';
import HormonesPopover from '@/components/wheel/popovers/mitigation/HormonesPopover.vue';
import MedicationReviewPopover from '@/components/wheel/popovers/mitigation/MedicationReviewPopover.vue';
import PreviousEyeSurgeryPopover from '@/components/wheel/popovers/mitigation/PreviousEyeSurgeryPopover.vue';
import ProactiveManagementOfOcularSurfaceDiseasePopover from '@/components/wheel/popovers/mitigation/ProactiveManagementOfOcularSurfaceDiseasePopover.vue';
import CornealSensitivityAssessmentPopover from '@/components/wheel/popovers/mitigation/CornealSensitivityAssessmentPopover.vue';

const controlsStore = useControlsStore();
</script>

<template>
    <MitigationPopover
        v-if="
            controlsStore.selectedArea === 'mitigation' && !controlsStore.selectedSection && !controlsStore.selectedItem
        " />

    <!-- Section Popovers -->
    <QuestionnaireForEarlyIdPopover v-if="controlsStore.selectedItem === 'questionnaire'" />
    <DifferentialDiagnosisPopover v-if="controlsStore.selectedItem === 'differential-diagnosis'" />
    <ProphylaxisPopover v-if="controlsStore.selectedItem === 'prophylaxis'" />
    <SleepPopover v-if="controlsStore.selectedItem === 'sleep'" />
    <ContactLensesPopover v-if="controlsStore.selectedItem === 'contact-lens'" />
    <DigitalEyeStrainPopover v-if="controlsStore.selectedItem === 'digital-eye-strain'" />
    <EnvironmentPopover v-if="controlsStore.selectedItem === 'environment'" />
    <HormonesPopover v-if="controlsStore.selectedItem === 'hormones'" />
    <MedicationReviewPopover v-if="controlsStore.selectedItem === 'medication-review'" />
    <PreviousEyeSurgeryPopover v-if="controlsStore.selectedItem === 'previous-eye-surgery'" />
    <ProactiveManagementOfOcularSurfaceDiseasePopover
        v-if="controlsStore.selectedItem === 'proactive-management-of-ocular-surface-disease'" />
    <CornealSensitivityAssessmentPopover v-if="controlsStore.selectedItem === 'corneal-sensitivity-assessment'" />
</template>
