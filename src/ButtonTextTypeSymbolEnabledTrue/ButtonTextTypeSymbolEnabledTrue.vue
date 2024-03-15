<script setup>
import { defineProps } from "vue";
import ButtonProperty1MediumProperty2GhostProperty3DefaultProperty4IconOnly from "../ButtonProperty1MediumProperty2GhostProperty3DefaultProperty4IconOnly/ButtonProperty1MediumProperty2GhostProperty3DefaultProperty4IconOnly.vue";
import CircleDashed from "../CircleDashed/CircleDashed.vue";

defineProps({
  label: {
    type: String,
    default: "Link",
  },
  type: {
    type: String,
    default: "symbol",
  },
  enabled: {
    type: String,
    default: "false",
  },
});
</script>

<template>
  <div
    :class="
      'button-text-type-symbol-enabled-true ' +
      'type-' +
      type +
      ' enabled-' +
      enabled
    "
  >
    <slot name="icon">
      <ButtonProperty1MediumProperty2GhostProperty3DefaultProperty4IconOnly
        property2="ghost"
        property4="icon-only"
        class="button-instance"
      >
        <template #iconInstance>
          <CircleDashed class="circle-dashed-instance"></CircleDashed>
        </template>
      </ButtonProperty1MediumProperty2GhostProperty3DefaultProperty4IconOnly>
    </slot>
  </div>
</template>

<style scoped>
.button-text-type-symbol-enabled-true,
.button-text-type-symbol-enabled-true * {
  box-sizing: border-box;
}
.button-text-type-symbol-enabled-true {
  display: flex;
  flex-direction: row;
  gap: var(--spacing-10, 0.625rem);
  align-items: flex-start;
  justify-content: flex-start;
  position: relative;
}

/* nested override styles */
.circle-dashed-instance {
  align-self: stretch !important;
  flex: 1 !important;
  height: auto !important;
  width: unset !important;
}
.button-instance {
  flex-shrink: 0 !important;
}
</style>
