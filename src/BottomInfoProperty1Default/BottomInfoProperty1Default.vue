<script setup>
import { defineProps } from "vue";
import BubbleInformationProperty1Assistant from "../BubbleInformationProperty1Assistant/BubbleInformationProperty1Assistant.vue";
import CopyWeightRegular from "../CopyWeightRegular/CopyWeightRegular.vue";

defineProps({
  property1: {
    type: String,
    default: "default",
  },
});
</script>

<template>
  <div :class="'bottom-info-property-1-default ' + 'property-1-' + property1">
    <BubbleInformationProperty1Assistant
      class="bubble-information-instance"
    ></BubbleInformationProperty1Assistant>
    <CopyWeightRegular class="copy-instance"></CopyWeightRegular>
  </div>
</template>

<style scoped>
.bottom-info-property-1-default,
.bottom-info-property-1-default * {
  box-sizing: border-box;
}
.bottom-info-property-1-default {
  padding: 0.625rem;
  display: flex;
  flex-direction: row;
  align-items: center;
  justify-content: space-between;
  position: relative;
}
.bubble-information-instance {
  flex-shrink: 0 !important;
}
.copy-instance {
  flex-shrink: 0 !important;
}
</style>
