<script setup>
import { defineProps } from "vue";
import CircleDashed from "../CircleDashed/CircleDashed.vue";
import ButtonProperty1MediumProperty2GhostProperty3DefaultProperty4IconOnly from "../ButtonProperty1MediumProperty2GhostProperty3DefaultProperty4IconOnly/ButtonProperty1MediumProperty2GhostProperty3DefaultProperty4IconOnly.vue";

defineProps({
  buttons: {
    type: String,
    default: "2",
  },
});
</script>

<template>
  <div :class="'controls-trailing-buttons-buttons-2 ' + 'buttons-' + buttons">
    <slot name="component0">
      <ButtonProperty1MediumProperty2GhostProperty3DefaultProperty4IconOnly
        property2="ghost"
        property4="icon-only"
        class="trailing-button-1-instance"
      >
        <template #iconInstance>
          <CircleDashed class="circle-dashed-instance"></CircleDashed>
        </template>
      </ButtonProperty1MediumProperty2GhostProperty3DefaultProperty4IconOnly>
    </slot>
    <slot name="component1">
      <ButtonProperty1MediumProperty2GhostProperty3DefaultProperty4IconOnly
        property2="ghost"
        property4="icon-only"
        class="trailing-button-1-instance"
      >
        <template #iconInstance>
          <CircleDashed class="circle-dashed-instance"></CircleDashed>
        </template>
      </ButtonProperty1MediumProperty2GhostProperty3DefaultProperty4IconOnly>
    </slot>
  </div>
</template>

<style scoped>
.controls-trailing-buttons-buttons-2,
.controls-trailing-buttons-buttons-2 * {
  box-sizing: border-box;
}
.controls-trailing-buttons-buttons-2 {
  padding: 0.6875rem var(--spacing-16, 1rem) 0.6875rem 0rem;
  display: flex;
  flex-direction: row;
  gap: var(--spacing-16, 1rem);
  align-items: center;
  justify-content: flex-end;
  position: relative;
}
.trailing-button-1-instance {
  flex-shrink: 0 !important;
}

/* nested override styles */
.circle-dashed-instance {
  align-self: stretch !important;
  flex: 1 !important;
  height: auto !important;
  width: unset !important;
}
</style>
