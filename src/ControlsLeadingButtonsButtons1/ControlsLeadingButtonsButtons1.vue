<script setup>
import { defineProps } from "vue";
import ButtonProperty1MediumProperty2GhostProperty3DefaultProperty4IconOnly from "../ButtonProperty1MediumProperty2GhostProperty3DefaultProperty4IconOnly/ButtonProperty1MediumProperty2GhostProperty3DefaultProperty4IconOnly.vue";
import CircleDashed from "../CircleDashed/CircleDashed.vue";
import ButtonTextTypeSymbolEnabledTrue from "../ButtonTextTypeSymbolEnabledTrue/ButtonTextTypeSymbolEnabledTrue.vue";

defineProps({
  buttons: {
    type: String,
    default: "2",
  },
});
</script>

<template>
  <div :class="'controls-leading-buttons-buttons-1 ' + 'buttons-' + buttons">
    <ButtonTextTypeSymbolEnabledTrue
      enabled="true"
      class="leading-button-1-instance"
    >
      <template #icon>
        <ButtonProperty1MediumProperty2GhostProperty3DefaultProperty4IconOnly
          class="button-instance"
          label="Button"
          property1="medium"
          property2="ghost"
          property3="default"
          property4="icon-only"
        >
          <template #iconInstance>
            <CircleDashed class="circle-dashed-instance"></CircleDashed>
          </template>
        </ButtonProperty1MediumProperty2GhostProperty3DefaultProperty4IconOnly>
      </template>
    </ButtonTextTypeSymbolEnabledTrue>
  </div>
</template>

<style scoped>
.controls-leading-buttons-buttons-1,
.controls-leading-buttons-buttons-1 * {
  box-sizing: border-box;
}
.controls-leading-buttons-buttons-1 {
  padding: 0.6875rem 0rem 0.6875rem var(--spacing-16, 1rem);
  display: flex;
  flex-direction: row;
  gap: var(--spacing-16, 1rem);
  align-items: center;
  justify-content: flex-start;
  position: relative;
}
.leading-button-1-instance {
  flex-shrink: 0 !important;
}

/* nested override styles */
.circle-dashed-instance {
  align-self: stretch !important;
  flex: 1 !important;
  height: auto !important;
  width: unset !important;
}
.button-instance {
  background: var(--translucid-transparent, rgba(255, 255, 255, 0)) !important;
  flex-shrink: 0 !important;
}
</style>
