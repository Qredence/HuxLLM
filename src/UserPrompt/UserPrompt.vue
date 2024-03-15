<script setup>
import { defineProps } from "vue";
import PaperPlaneTiltWeightBold from "../PaperPlaneTiltWeightBold/PaperPlaneTiltWeightBold.vue";
import PaperPlaneTiltWeightRegular from "../PaperPlaneTiltWeightRegular/PaperPlaneTiltWeightRegular.vue";
import ButtonModeLightSizeMediumStyleBezeledGrayStateEnabledOnMaterialTrueLabelTypeSymbolText from "../ButtonModeLightSizeMediumStyleBezeledGrayStateEnabledOnMaterialTrueLabelTypeSymbolText/ButtonModeLightSizeMediumStyleBezeledGrayStateEnabledOnMaterialTrueLabelTypeSymbolText.vue";

defineProps({});
</script>

<template>
  <div class="user-prompt">
    <div class="value">Ask a question</div>
    <ButtonModeLightSizeMediumStyleBezeledGrayStateEnabledOnMaterialTrueLabelTypeSymbolText
      label="Send"
      size="medium"
      styleVariant="bezeled-gray"
      onMaterial="true"
      class="button-instance"
    >
      <template #component0>
        <PaperPlaneTiltWeightBold
          class="paper-plane-tilt-instance"
          weight="bold"
        ></PaperPlaneTiltWeightBold>
      </template>
    </ButtonModeLightSizeMediumStyleBezeledGrayStateEnabledOnMaterialTrueLabelTypeSymbolText>
  </div>
</template>

<style scoped>
.user-prompt,
.user-prompt * {
  box-sizing: border-box;
}
.user-prompt {
  background: var(--background-background-container, #fcfcfc);
  border-radius: 0.75rem;
  border-style: solid;
  border-color: var(--container-surface-primary, rgba(120, 120, 128, 0.2));
  border-width: 0.0625rem;
  padding: 0rem 0.5rem 0rem 1.25rem;
  display: flex;
  flex-direction: row;
  gap: 0rem;
  align-items: center;
  justify-content: flex-start;
  height: 3.5rem;
  position: relative;
  box-shadow: var(
    --shadows-shadow-l-box-shadow,
    0rem 0.25rem 1.3125rem 0rem rgba(0, 0, 0, 0.05)
  );
  overflow: hidden;
}
.value {
  color: var(--text-text-secondary, rgba(0, 0, 0, 0.5));
  text-align: left;
  font-family: var(--body-font-family, "SfPro-Medium", sans-serif);
  font-size: var(--body-font-size, 1.0625rem);
  line-height: var(--body-line-height, 1.375rem);
  font-weight: var(--body-font-weight, 500);
  position: relative;
  flex: 1;
  display: flex;
  align-items: center;
  justify-content: flex-start;
  text-overflow: ellipsis;
  overflow: hidden;
  white-space: nowrap;
}
.button-instance {
  flex-shrink: 0 !important;
}

/* nested override styles */
.paper-plane-tilt-instance {
  flex-shrink: 0 !important;
  width: 1rem !important;
  height: 1rem !important;
}
</style>
