<script setup>
import { defineProps } from "vue";
import Date from "../Date/Date.vue";
import Thumbs from "../Thumbs/Thumbs.vue";

defineProps({});
</script>

<template>
  <div class="left-information">
    <Date class="date-instance"></Date>
    <Thumbs class="thumbs-instance"></Thumbs>
  </div>
</template>

<style scoped>
.left-information,
.left-information * {
  box-sizing: border-box;
}
.left-information {
  display: flex;
  flex-direction: row;
  gap: 0.875rem;
  align-items: center;
  justify-content: flex-start;
  position: relative;
}
.date-instance {
  flex-shrink: 0 !important;
}
.thumbs-instance {
  flex-shrink: 0 !important;
}
</style>
