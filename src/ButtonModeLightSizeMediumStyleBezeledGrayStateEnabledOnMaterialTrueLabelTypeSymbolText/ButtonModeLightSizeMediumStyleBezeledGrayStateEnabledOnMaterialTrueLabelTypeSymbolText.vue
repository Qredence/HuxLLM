<script setup>
import { defineProps } from "vue";
import PaperPlaneTiltWeightRegular from "../PaperPlaneTiltWeightRegular/PaperPlaneTiltWeightRegular.vue";

defineProps({
  label: {
    type: String,
    default: "Play",
  },
  mode: {
    type: String,
    default: "light",
  },
  size: {
    type: String,
    default: "small",
  },
  styleVariant: {
    type: String,
    default: "borderless",
  },
  state: {
    type: String,
    default: "enabled",
  },
  onMaterial: {
    type: String,
    default: "false",
  },
  labelType: {
    type: String,
    default: "symbol-text",
  },
});
</script>

<template>
  <div
    :class="
      'button-mode-light-size-medium-style-bezeled-gray-state-enabled-on-material-true-label-type-symbol-text ' +
      'mode-' +
      mode +
      ' size-' +
      size +
      ' style-variant-' +
      styleVariant +
      ' state-' +
      state +
      ' on-material-' +
      onMaterial +
      ' label-type-' +
      labelType
    "
  >
    <div class="label">
      {{ label }}
    </div>
    <slot name="component0">
      <PaperPlaneTiltWeightRegular
        class="paper-plane-tilt-instance"
      ></PaperPlaneTiltWeightRegular>
    </slot>
  </div>
</template>

<style scoped>
.button-mode-light-size-medium-style-bezeled-gray-state-enabled-on-material-true-label-type-symbol-text,
.button-mode-light-size-medium-style-bezeled-gray-state-enabled-on-material-true-label-type-symbol-text
  * {
  box-sizing: border-box;
}
.button-mode-light-size-medium-style-bezeled-gray-state-enabled-on-material-true-label-type-symbol-text {
  background: var(--fills-tertiary, rgba(118, 118, 128, 0.12));
  border-radius: 2.5rem;
  padding: 0.4375rem 0.875rem 0.4375rem 0.875rem;
  display: flex;
  flex-direction: row;
  gap: 0.25rem;
  align-items: center;
  justify-content: center;
  position: relative;
}
.label {
  color: var(--colors-blue, #007aff);
  text-align: left;
  font-family: var(
    --subheadline-regular-font-family,
    "SfPro-Regular",
    sans-serif
  );
  font-size: var(--subheadline-regular-font-size, 0.9375rem);
  line-height: var(--subheadline-regular-line-height, 1.25rem);
  font-weight: var(--subheadline-regular-font-weight, 400);
  position: relative;
}
.paper-plane-tilt-instance {
  flex-shrink: 0 !important;
  width: 1rem !important;
  height: 1rem !important;
}
</style>
