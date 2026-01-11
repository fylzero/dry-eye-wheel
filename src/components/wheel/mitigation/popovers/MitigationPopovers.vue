<script setup>
import { useControlsStore } from '@/stores/controlsStore.js';
import MitigationPopover from '@/components/wheel/mitigation/popovers/MitigationPopover.vue';
import QuestionnaireForEarlyIdPopover from '@/components/wheel/mitigation/popovers/QuestionnaireForEarlyIdPopover.vue';
import DifferentialDiagnosisPopover from '@/components/wheel/mitigation/popovers/DifferentialDiagnosisPopover.vue';
import ProphylaxisPopover from '@/components/wheel/mitigation/popovers/ProphylaxisPopover.vue';
import SleepPopover from '@/components/wheel/mitigation/popovers/SleepPopover.vue';
import ContactLensesPopover from '@/components/wheel/mitigation/popovers/ContactLensesPopover.vue';
import DigitalEyeStrainPopover from '@/components/wheel/mitigation/popovers/DigitalEyeStrainPopover.vue';
import EnvironmentPopover from '@/components/wheel/mitigation/popovers/EnvironmentPopover.vue';
import HormonesPopover from '@/components/wheel/mitigation/popovers/HormonesPopover.vue';
import MedicationReviewPopover from '@/components/wheel/mitigation/popovers/MedicationReviewPopover.vue';
import PreviousEyeSurgeryPopover from '@/components/wheel/mitigation/popovers/PreviousEyeSurgeryPopover.vue';
import ProactiveManagementOfOcularSurfaceDiseasePopover from '@/components/wheel/mitigation/popovers/ProactiveManagementOfOcularSurfaceDiseasePopover.vue';
import CornealSensitivityAssessmentPopover from '@/components/wheel/mitigation/popovers/CornealSensitivityAssessmentPopover.vue';

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
