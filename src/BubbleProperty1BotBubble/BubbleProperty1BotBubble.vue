<script setup>
import { defineProps } from "vue";
defineProps({
  message: {
    type: String,
    default:
      "Why Qream UI?Figma&#039;s Latest Features: Stay ahead of the competition with our pioneering use of Figma&#039;s modern features like variables. Streamline your design process with reusable, dynamic components.Apple Design: Qream UI utilizes the sleek and intuitive Apple Design language to enhance user engagement and interaction.For Designers and Developers: Our UI Kit serves as a comprehensive toolkit for both designers and developers, facilitating efficient design handoff and smoothing the transition from design to code.",
  },
  property1: {
    type: String,
    default: "bot-bubble",
  },
});
</script>

<template>
  <div :class="'bubble-property-1-bot-bubble ' + 'property-1-' + property1">
    <div class="heading">
      {{ message }}
    </div>
  </div>
</template>

<style scoped>
.bubble-property-1-bot-bubble,
.bubble-property-1-bot-bubble * {
  box-sizing: border-box;
}
.bubble-property-1-bot-bubble {
  background: var(--chatwindowtheme-backgroundcolor, #fcfcfc);
  border-radius: var(--radius-radius-l, 1.5rem);
  padding: var(--spacing-16, 1rem) var(--spacing-24, 1.5rem)
    var(--spacing-24, 1.5rem) var(--spacing-24, 1.5rem);
  display: flex;
  flex-direction: column;
  gap: var(--spacing-16, 1rem);
  align-items: center;
  justify-content: center;
  flex-shrink: 0;
  position: relative;
  box-shadow: 0rem 0rem 0.65rem 0rem rgba(0, 0, 0, 0.19);
}
.heading {
  color: var(--text-text-primary, rgba(0, 0, 0, 0.85));
  text-align: left;
  font-family: var(--body-emphasized-font-family, "SfPro-Semibold", sans-serif);
  font-size: var(--body-emphasized-font-size, 1.0625rem);
  line-height: var(--body-emphasized-line-height, 1.375rem);
  font-weight: var(--body-emphasized-font-weight, 600);
  position: relative;
  align-self: stretch;
}
</style>
