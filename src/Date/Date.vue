<script setup>
import { defineProps } from "vue";
defineProps({});
</script>

<template>
  <div class="date">
    <div class="date2">15:15</div>
  </div>
</template>

<style scoped>
.date,
.date * {
  box-sizing: border-box;
}
.date {
  padding: 0.5625rem 0rem 0.5625rem 0rem;
  display: flex;
  flex-direction: row;
  gap: 0.625rem;
  align-items: center;
  justify-content: center;
  position: relative;
}
.date2 {
  color: var(--text-text-primary, rgba(0, 0, 0, 0.85));
  text-align: left;
  font-family: var(--body-emphasized-font-family, "SfPro-Semibold", sans-serif);
  font-size: var(--body-emphasized-font-size, 1.0625rem);
  line-height: var(--body-emphasized-line-height, 1.375rem);
  font-weight: var(--body-emphasized-font-weight, 600);
  position: relative;
  display: flex;
  align-items: center;
  justify-content: flex-start;
}
</style>
