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
  <div :class="'avatar-src-role-user ' + 'role-' + role">
    <div class="avatar">
      <div class="circle"></div>
      <div class="z">Z</div>
    </div>
  </div>
</template>

<style scoped>
.avatar-src-role-user,
.avatar-src-role-user * {
  box-sizing: border-box;
}
.avatar-src-role-user {
  background: var(--surface-div-primary, rgba(0, 0, 0, 0.85));
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
.z {
  color: var(--background-background-container, #fcfcfc);
  text-align: left;
  font-family: "Inter-Bold", sans-serif;
  font-size: 1.75rem;
  line-height: 2.5rem;
  font-weight: 700;
  position: absolute;
  left: 0.9375rem;
  top: 0.25rem;
  display: flex;
  align-items: center;
  justify-content: flex-start;
}
</style>
