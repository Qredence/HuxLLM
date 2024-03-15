<script setup>
import { defineProps } from "vue";
import BubbleProperty1BotBubble from "../BubbleProperty1BotBubble/BubbleProperty1BotBubble.vue";
import BottomInfoProperty1Default from "../BottomInfoProperty1Default/BottomInfoProperty1Default.vue";

defineProps({
  property1: {
    type: String,
    default: "assistant",
  },
});
</script>

<template>
  <div :class="'chat-bubble-property-1-assistant ' + 'property-1-' + property1">
    <BubbleProperty1BotBubble
      class="bubble-instance"
    ></BubbleProperty1BotBubble>
    <BottomInfoProperty1Default
      class="bottom-info-instance"
    ></BottomInfoProperty1Default>
  </div>
</template>

<style scoped>
.chat-bubble-property-1-assistant,
.chat-bubble-property-1-assistant * {
  box-sizing: border-box;
}
.chat-bubble-property-1-assistant {
  display: flex;
  flex-direction: column;
  gap: 1.4375rem;
  align-items: flex-end;
  justify-content: flex-start;
  flex: 1;
  position: relative;
}
.bubble-instance {
  align-self: stretch !important;
}
.bottom-info-instance {
  align-self: stretch !important;
  flex-shrink: 0 !important;
}
</style>
