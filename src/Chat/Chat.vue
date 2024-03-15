<script setup>
import { defineProps } from "vue";
import NavigationBarIPad from "../NavigationBarIPad/NavigationBarIPad.vue";
import ChatBubbleProperty1Assistant from "../ChatBubbleProperty1Assistant/ChatBubbleProperty1Assistant.vue";
import ChatBubbleProperty1User from "../ChatBubbleProperty1User/ChatBubbleProperty1User.vue";
import UserPrompt from "../UserPrompt/UserPrompt.vue";
</script>

<template>
  <div class="chat">
    <NavigationBarIPad
      class="navigation-bar-i-pad-instance"
    ></NavigationBarIPad>
    <div class="body">
      <div class="container">
        <ChatBubbleProperty1Assistant
          class="chat-bubble-instance"
        ></ChatBubbleProperty1Assistant>
        <ChatBubbleProperty1User
          property1="user"
          class="chat-bubble-instance"
        ></ChatBubbleProperty1User>
      </div>
      <div class="input-wrapper">
        <UserPrompt class="user-prompt-instance"></UserPrompt>
      </div>
    </div>
  </div>
</template>

<style scoped>
.chat,
.chat * {
  box-sizing: border-box;
}
.chat {
  background: var(--background-background-page, #ffffff);
  display: flex;
  flex-direction: column;
  gap: var(--spacing-0, 0rem);
  align-items: center;
  justify-content: flex-start;
  height: 59.25rem;
  position: relative;
  overflow: hidden;
}
.navigation-bar-i-pad-instance {
  flex-shrink: 0 !important;
  background: unset !important;
}
.body {
  padding: 0rem 0rem 3.5rem 0rem;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: space-between;
  align-self: stretch;
  flex-shrink: 0;
  height: 53.875rem;
  position: relative;
}
.container {
  padding: 1.5rem var(--spacing-10, 0.625rem) 1.625rem
    var(--spacing-10, 0.625rem);
  display: flex;
  flex-direction: column;
  gap: 1.5rem;
  align-items: center;
  justify-content: flex-start;
  width: 100%;
  flex-shrink: 0;
  min-width: 24.375rem;
  max-width: 47.75rem;
  position: relative;
  overflow-y: auto;
}
.chat-bubble-instance {
  align-self: stretch !important;
  flex-shrink: 0 !important;
  flex: unset !important;
}
.input-wrapper {
  display: flex;
  flex-direction: column;
  gap: 0.625rem;
  align-items: flex-start;
  justify-content: center;
  flex-shrink: 0;
  width: 57.375rem;
  height: 3.5rem;
  position: relative;
}
.user-prompt-instance {
  align-self: stretch !important;
  flex-shrink: 0 !important;
}
</style>
