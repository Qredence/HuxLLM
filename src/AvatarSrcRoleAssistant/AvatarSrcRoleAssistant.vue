<script setup>
import { defineProps } from "vue";
defineProps({
  role: {
    type: String,
    default: "assistant",
  },
});
</script>

<template>
  <div :class="'avatar-src-role-assistant ' + 'role-' + role">
    <div class="avatar">
      <div class="circle"></div>
      <div class="b">B</div>
    </div>
  </div>
</template>

<style scoped>
.avatar-src-role-assistant,
.avatar-src-role-assistant * {
  box-sizing: border-box;
}
.avatar-src-role-assistant {
  background: var(--container-surface-primary, rgba(120, 120, 128, 0.2));
  border-radius: var(--numeric-31.25rem, 31.25rem);
  width: 3rem;
  height: 3rem;
  position: relative;
  overflow: hidden;
}
.avatar {
  width: 3rem;
  height: 3rem;
  position: absolute;
  left: 0rem;
  top: 0rem;
}
.circle {
  border-radius: 50%;
  width: 3rem;
  height: 3rem;
  position: absolute;
  left: 0rem;
  top: 0rem;
}
.b {
  color: var(--color-primarycolor, #007aff);
  text-align: left;
  font-family: "Inter-SemiBold", sans-serif;
  font-size: 1.75rem;
  line-height: 2.5rem;
  font-weight: 600;
  position: absolute;
  left: 0.9375rem;
  top: 0.25rem;
  display: flex;
  align-items: center;
  justify-content: flex-start;
}
</style>
