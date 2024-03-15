<script setup>
import { defineProps } from "vue";
import AvatarSrcRoleAssistant from "../AvatarSrcRoleAssistant/AvatarSrcRoleAssistant.vue";
import LeftInformation from "../LeftInformation/LeftInformation.vue";

defineProps({
  property1: {
    type: String,
    default: "assistant",
  },
});
</script>

<template>
  <div
    :class="
      'bubble-information-property-1-assistant ' + 'property-1-' + property1
    "
  >
    <AvatarSrcRoleAssistant
      class="avatar-src-instance"
    ></AvatarSrcRoleAssistant>
    <LeftInformation class="left-information-instance"></LeftInformation>
  </div>
</template>

<style scoped>
.bubble-information-property-1-assistant,
.bubble-information-property-1-assistant * {
  box-sizing: border-box;
}
.bubble-information-property-1-assistant {
  display: flex;
  flex-direction: row;
  gap: 1rem;
  align-items: center;
  justify-content: flex-start;
  position: relative;
}
.avatar-src-instance {
  flex-shrink: 0 !important;
}
.left-information-instance {
  flex-shrink: 0 !important;
}
</style>
