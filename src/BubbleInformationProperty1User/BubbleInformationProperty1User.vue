<script setup>
import { defineProps } from "vue";
import AvatarSrcRoleUser from "../AvatarSrcRoleUser/AvatarSrcRoleUser.vue";
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
    :class="'bubble-information-property-1-user ' + 'property-1-' + property1"
  >
    <AvatarSrcRoleUser
      role="user"
      class="avatar-src-instance"
    ></AvatarSrcRoleUser>
    <LeftInformation class="left-information-instance"></LeftInformation>
  </div>
</template>

<style scoped>
.bubble-information-property-1-user,
.bubble-information-property-1-user * {
  box-sizing: border-box;
}
.bubble-information-property-1-user {
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
