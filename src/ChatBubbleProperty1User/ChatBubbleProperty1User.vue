<script setup>
import { defineProps } from "vue";
import BubbleProperty1UserBubble from "../BubbleProperty1UserBubble/BubbleProperty1UserBubble.vue";
import BubbleInformationProperty1User from "../BubbleInformationProperty1User/BubbleInformationProperty1User.vue";
import BubbleInformationProperty1Assistant from "../BubbleInformationProperty1Assistant/BubbleInformationProperty1Assistant.vue";
import BottomInfoProperty1Default from "../BottomInfoProperty1Default/BottomInfoProperty1Default.vue";

defineProps({
  property1: {
    type: String,
    default: "assistant",
  },
});
</script>

<template>
  <div :class="'chat-bubble-property-1-user ' + 'property-1-' + property1">
    <BubbleProperty1UserBubble
      property1="user-bubble"
      class="bubble-instance"
    ></BubbleProperty1UserBubble>
    <BottomInfoProperty1Default class="bottom-info-instance">
      <template #component0>
        <BubbleInformationProperty1User
          class="bubble-information-instance"
          property1="user"
        ></BubbleInformationProperty1User>
      </template>
    </BottomInfoProperty1Default>
  </div>
</template>

<style scoped>
.chat-bubble-property-1-user,
.chat-bubble-property-1-user * {
  box-sizing: border-box;
}
.chat-bubble-property-1-user {
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

/* nested override styles */
.bubble-information-instance {
  flex-shrink: 0 !important;
}
</style>
