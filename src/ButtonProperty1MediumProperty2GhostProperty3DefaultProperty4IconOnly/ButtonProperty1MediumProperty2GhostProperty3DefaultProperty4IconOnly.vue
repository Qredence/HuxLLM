<script setup>
import { defineProps } from "vue";
import CircleDashed2 from "../CircleDashed2/CircleDashed2.vue";
import CircleDashed from "../CircleDashed/CircleDashed.vue";

defineProps({
  label: {
    type: String,
    default: "Button",
  },
  property1: {
    type: String,
    default: "medium",
  },
  property2: {
    type: String,
    default: "primary",
  },
  property3: {
    type: String,
    default: "default",
  },
  property4: {
    type: String,
    default: "icon-after",
  },
});
</script>

<template>
  <div
    :class="
      'button-property-1-medium-property-2-ghost-property-3-default-property-4-icon-only ' +
      'property-1-' +
      property1 +
      ' property-2-' +
      property2 +
      ' property-3-' +
      property3 +
      ' property-4-' +
      property4
    "
  >
    <slot name="iconInstance">
      <CircleDashed class="circle-dashed-instance"></CircleDashed>
    </slot>
  </div>
</template>

<style scoped>
.button-property-1-medium-property-2-ghost-property-3-default-property-4-icon-only,
.button-property-1-medium-property-2-ghost-property-3-default-property-4-icon-only
  * {
  box-sizing: border-box;
}
.button-property-1-medium-property-2-ghost-property-3-default-property-4-icon-only {
  border-radius: var(--radius-radius-xs, 0.5rem);
  padding: var(--spacing-4, 0.25rem);
  display: flex;
  flex-direction: row;
  gap: var(--spacing-4, 0.25rem);
  align-items: center;
  justify-content: center;
  width: 1.75rem;
  height: 1.75rem;
  position: relative;
}

/* nested override styles */
.circle-dashed-instance {
  align-self: stretch !important;
  flex: 1 !important;
  height: auto !important;
  width: unset !important;
}
</style>
