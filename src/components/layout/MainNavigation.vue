<script setup>
import { storeToRefs } from 'pinia';
import { watch } from 'vue';
import { useControlsStore } from '../../stores/controlsStore.js';
import GradientButton from '../GradientButton.vue';

const controlsStore = useControlsStore();
const { sliderValue } = storeToRefs(controlsStore);

watch(sliderValue, () => {
    if (sliderValue.value === 0) {
        document.getElementById('scroll-me').scrollTo({
            top: 0,
            behavior: 'smooth',
        });
    }
    if (sliderValue.value === 50) {
        document.getElementById('scroll-me').scrollTo({
            top: 392,
            behavior: 'smooth',
        });
    }
    if (sliderValue.value === 100) {
        document.getElementById('scroll-me').scrollTo({
            top: 760,
            behavior: 'smooth',
        });
    }
});
</script>

<template>
    <div
        id="scroll-me"
        class="mx-6 flex w-full flex-col gap-3 overflow-y-hidden p-[3px]">
        <!-- Mitigation -->
        <GradientButton
            id="mitigation-area"
            @click="controlsStore.selectArea('mitigation')"
            :class="{ active: controlsStore.selectedArea === 'mitigation' }"
            class="btn-area">
            {{ $t('Mitigation') }}
        </GradientButton>
        <div class="grid grid-cols-2 gap-3">
            <GradientButton
                @click="controlsStore.selectSection('risk-factors', 'mitigation')"
                :class="{ active: controlsStore.selectedSection === 'risk-factors' }"
                class="btn-section">
                {{ $t('Risk Factors') }}
            </GradientButton>
            <GradientButton
                @click="controlsStore.selectSection('triaging', 'mitigation')"
                :class="{ active: controlsStore.selectedSection === 'triaging' }"
                class="btn-section">
                {{ $t('Triaging') }}
            </GradientButton>
        </div>
        <div class="grid grid-cols-2 gap-3">
            <GradientButton
                @click="controlsStore.selectItem('sleep', 'risk-factors', 'mitigation')"
                :class="{ active: controlsStore.selectedItem === 'sleep' }"
                class="btn-orange">
                {{ $t('Sleep') }}
            </GradientButton>
            <GradientButton
                @click="controlsStore.selectItem('symptom-check', 'triaging', 'mitigation')"
                :class="{ active: controlsStore.selectedItem === 'symptom-check' }"
                class="btn-orange">
                {{ $t('Symptom Check') }}
            </GradientButton>
        </div>
        <div class="grid grid-cols-2 gap-3">
            <GradientButton
                @click="controlsStore.selectItem('contact-lens', 'risk-factors', 'mitigation')"
                :class="{ active: controlsStore.selectedItem === 'contact-lens' }"
                class="btn-orange">
                {{ $t('Contact Lens') }}
            </GradientButton>
            <GradientButton
                @click="controlsStore.selectItem('differential-diagnosis', 'triaging', 'mitigation')"
                :class="{ active: controlsStore.selectedItem === 'differential-diagnosis' }"
                class="btn-orange">
                {{ $t('Differential Diagnosis') }}
            </GradientButton>
        </div>
        <div class="grid grid-cols-2 gap-3">
            <GradientButton
                @click="controlsStore.selectItem('environment-advice', 'risk-factors', 'mitigation')"
                :class="{ active: controlsStore.selectedItem === 'environment-advice' }"
                class="btn-orange">
                {{ $t('Environment Advice') }}
            </GradientButton>
            <GradientButton
                @click="controlsStore.selectItem('digital-eye-strain', 'risk-factors', 'mitigation')"
                :class="{ active: controlsStore.selectedItem === 'digital-eye-strain' }"
                class="btn-orange">
                {{ $t('Digital Eye Strain') }}
            </GradientButton>
        </div>
        <div class="grid grid-cols-2 gap-3">
            <GradientButton
                @click="controlsStore.selectItem('previous-eye-surgery', 'risk-factors', 'mitigation')"
                :class="{ active: controlsStore.selectedItem === 'previous-eye-surgery' }"
                class="btn-silver">
                {{ $t('Previous Eye Surgery') }}
            </GradientButton>
            <GradientButton
                @click="
                    controlsStore.selectItem('proactive-management-of-ocular-surface-disease', 'triaging', 'mitigation')
                "
                :class="{ active: controlsStore.selectedItem === 'proactive-management-of-ocular-surface-disease' }"
                class="btn-silver">
                {{ $t('Proactive Management of Ocular Surface Disease') }}
            </GradientButton>
        </div>
        <div class="grid grid-cols-2 gap-3">
            <GradientButton
                @click="controlsStore.selectItem('hormones', 'risk-factors', 'mitigation')"
                :class="{ active: controlsStore.selectedItem === 'hormones' }"
                class="btn-silver">
                {{ $t('Hormones') }}
            </GradientButton>
            <GradientButton
                @click="controlsStore.selectItem('corneal-sensitivity-assessment', 'risk-factors', 'mitigation')"
                :class="{ active: controlsStore.selectedItem === 'corneal-sensitivity-assessment' }"
                class="btn-silver">
                {{ $t('Corneal Sensitivity Assessment') }}
            </GradientButton>
        </div>
        <div class="mb-6 grid grid-cols-2 gap-3">
            <GradientButton
                @click="controlsStore.selectItem('medication-review', 'risk-factors', 'mitigation')"
                :class="{ active: controlsStore.selectedItem === 'medication-review' }"
                class="btn-yellow">
                {{ $t('Medication Review') }}
            </GradientButton>
            <GradientButton
                @click="controlsStore.selectItem('prophylaxis', 'triaging', 'mitigation')"
                :class="{ active: controlsStore.selectedItem === 'prophylaxis' }"
                class="btn-yellow">
                {{ $t('Prophylaxis') }}
            </GradientButton>
        </div>

        <!-- Measurement -->
        <GradientButton
            id="measurement-area"
            @click="controlsStore.selectArea('measurement')"
            :class="{ active: controlsStore.selectedArea === 'measurement' }"
            class="btn-area">
            {{ $t('Measurement') }}
        </GradientButton>
        <div class="grid grid-cols-2 gap-3">
            <GradientButton
                @click="controlsStore.selectSection('diagnosis', 'measurement')"
                :class="{ active: controlsStore.selectedSection === 'diagnosis' }"
                class="btn-section">
                {{ $t('Diagnosis') }}
            </GradientButton>
            <GradientButton
                @click="controlsStore.selectSection('sub-typing', 'measurement')"
                :class="{ active: controlsStore.selectedSection === 'sub-typing' }"
                class="btn-section">
                {{ $t('Sub-Typing') }}
            </GradientButton>
        </div>
        <div class="grid grid-cols-2 gap-3">
            <GradientButton
                @click="controlsStore.selectItem('comfort-time-after-blink-test', 'diagnosis', 'measurement')"
                :class="{ active: controlsStore.selectedItem === 'comfort-time-after-blink-test' }"
                class="btn-orange">
                {{ $t('Comfort Time After Blink Test') }}
            </GradientButton>
            <GradientButton
                @click="controlsStore.selectItem('blink-rate-and-completeness', 'sub-typing', 'measurement')"
                :class="{ active: controlsStore.selectedItem === 'blink-rate-and-completeness' }"
                class="btn-orange">
                {{ $t('Blink Completeness and Lid Closure; Redness') }}
            </GradientButton>
        </div>
        <div class="grid grid-cols-2 gap-3">
            <GradientButton
                @click="controlsStore.selectItem('osdi-6', 'diagnosis', 'measurement')"
                :class="{ active: controlsStore.selectedItem === 'osdi-6' }"
                class="btn-orange">
                {{ $t('OSDI-6') }}
            </GradientButton>
            <GradientButton
                @click="controlsStore.selectItem('ocular-surface-misalignment', 'sub-typing', 'measurement')"
                :class="{ active: controlsStore.selectedItem === 'ocular-surface-misalignment' }"
                class="btn-silver">
                {{ $t('Ocular Surface Misalignment') }}
            </GradientButton>
        </div>
        <div class="grid grid-cols-2 gap-3">
            <GradientButton
                @click="controlsStore.selectItem('aqueous-tear-meniscus-height', 'sub-typing', 'measurement')"
                :class="{ active: controlsStore.selectedItem === 'aqueous-tear-meniscus-height' }"
                class="btn-silver">
                {{ $t('Aqueous Tear Meniscus Height') }}
            </GradientButton>
            <GradientButton
                @click="controlsStore.selectItem('fluorescein-staining', 'diagnosis', 'measurement')"
                :class="{ active: controlsStore.selectedItem === 'fluorescein-staining' }"
                class="btn-silver">
                {{ $t('Fluorescein Staining') }}
            </GradientButton>
        </div>
        <div class="grid grid-cols-2 gap-3">
            <GradientButton
                @click="controlsStore.selectItem('eyelids-meibomian-gland-expression', 'sub-typing', 'measurement')"
                :class="{ active: controlsStore.selectedItem === 'eyelids-meibomian-gland-expression' }"
                class="btn-silver">
                {{ $t('Eyelids: Meibomian Gland Expression') }}
            </GradientButton>
            <GradientButton
                @click="controlsStore.selectItem('eyelids-anterior-blepharitis-exam', 'sub-typing', 'measurement')"
                :class="{ active: controlsStore.selectedItem === 'eyelids-anterior-blepharitis-exam' }"
                class="btn-silver">
                {{ $t('Eyelids: Anterior Blepharitis Exam') }}
            </GradientButton>
        </div>
        <div class="grid grid-cols-2 gap-3">
            <GradientButton
                @click="controlsStore.selectItem('non-invasive-breakup-time', 'diagnosis', 'measurement')"
                :class="{ active: controlsStore.selectedItem === 'non-invasive-breakup-time' }"
                class="btn-silver">
                {{ $t('Non-Invasive Breakup Time') }}
            </GradientButton>
            <GradientButton
                @click="controlsStore.selectItem('meibography-and-interferometry', 'sub-typing', 'measurement')"
                :class="{ active: controlsStore.selectedItem === 'meibography-and-interferometry' }"
                class="btn-yellow">
                {{ $t('Meibography and Interferometry') }}
            </GradientButton>
        </div>
        <div class="grid grid-cols-2 gap-3">
            <GradientButton
                @click="controlsStore.selectItem('osmolarity', 'diagnosis', 'measurement')"
                :class="{ active: controlsStore.selectedItem === 'osmolarity' }"
                class="btn-silver">
                {{ $t('Osmolarity') }}
            </GradientButton>
            <GradientButton
                @click="controlsStore.selectItem('lissamine-green-staining', 'diagnosis', 'measurement')"
                :class="{ active: controlsStore.selectedItem === 'lissamine-green-staining' }"
                class="btn-yellow">
                {{ $t('Lissamine Green Staining') }}
            </GradientButton>
        </div>

        <!-- Management -->
        <GradientButton
            id="management-area"
            @click="controlsStore.selectArea('management')"
            :class="{ active: controlsStore.selectedArea === 'management' }"
            class="btn-area">
            {{ $t('Management') }}
        </GradientButton>
        <div class="grid grid-cols-2 gap-3">
            <GradientButton
                @click="controlsStore.selectItem('lid-hygiene', null, 'management')"
                :class="{ active: controlsStore.selectedItem === 'lid-hygiene' }"
                class="btn-orange">
                {{ $t('Lid Hygiene') }}
            </GradientButton>
            <GradientButton
                @click="controlsStore.selectItem('warm-compress', null, 'management')"
                :class="{ active: controlsStore.selectedItem === 'warm-compress' }"
                class="btn-orange">
                {{ $t('Warm Compress') }}
            </GradientButton>
        </div>
        <div class="grid grid-cols-2 gap-3">
            <GradientButton
                @click="controlsStore.selectItem('blink-exercises', null, 'management')"
                :class="{ active: controlsStore.selectedItem === 'blink-exercises' }"
                class="btn-orange">
                {{ $t('Blink Exercises') }}
            </GradientButton>
            <GradientButton
                @click="controlsStore.selectItem('advice', null, 'management')"
                :class="{ active: controlsStore.selectedItem === 'advice' }"
                class="btn-orange">
                {{ $t('Advice') }}
            </GradientButton>
        </div>
        <div class="grid grid-cols-2 gap-3">
            <GradientButton
                @click="controlsStore.selectItem('artificial-tears', null, 'management')"
                :class="{ active: controlsStore.selectedItem === 'artificial-tears' }"
                class="btn-orange">
                {{ $t('Artificial Tears') }}
            </GradientButton>
            <GradientButton
                @click="controlsStore.selectItem('diet-and-dietary-supplements', null, 'management')"
                :class="{ active: controlsStore.selectedItem === 'diet-and-dietary-supplements' }"
                class="btn-orange">
                {{ $t('Diet And Dietary Supplements') }}
            </GradientButton>
        </div>
        <div class="grid grid-cols-2 gap-3">
            <GradientButton
                @click="controlsStore.selectItem('scleral-lenses', null, 'management')"
                :class="{ active: controlsStore.selectedItem === 'scleral-lenses' }"
                class="btn-silver">
                {{ $t('Scleral Lenses') }}
            </GradientButton>
            <GradientButton
                @click="controlsStore.selectItem('pharmaceuticals', null, 'management')"
                :class="{ active: controlsStore.selectedItem === 'pharmaceuticals' }"
                class="btn-silver">
                {{ $t('Pharmaceuticals') }}
            </GradientButton>
        </div>
        <div class="grid grid-cols-2 gap-3">
            <GradientButton
                @click="controlsStore.selectItem('in-office-light-heat-based-devices', null, 'management')"
                :class="{ active: controlsStore.selectedItem === 'in-office-light-heat-based-devices' }"
                class="btn-silver">
                {{ $t('In-Office Light/Heat-Based Devices') }}
            </GradientButton>
            <GradientButton
                @click="controlsStore.selectItem('surgical-approaches', null, 'management')"
                :class="{ active: controlsStore.selectedItem === 'surgical-approaches' }"
                class="btn-yellow">
                {{ $t('Surgical Approaches') }}
            </GradientButton>
        </div>
        <div class="grid grid-cols-2 gap-3">
            <GradientButton
                @click="controlsStore.selectItem('complex-treatments', null, 'management')"
                :class="{ active: controlsStore.selectedItem === 'complex-treatments' }"
                class="btn-yellow">
                {{ $t('Complex Treatments') }}
            </GradientButton>
        </div>
        <!-- Empty space -->
        <div class="h-[600px]">
            <div class="h-[600px]">&nbsp;</div>
        </div>
    </div>
</template>
