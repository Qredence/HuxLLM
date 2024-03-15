<script setup>
import { defineProps } from "vue";
import ThumbsUpWeightRegular from "../ThumbsUpWeightRegular/ThumbsUpWeightRegular.vue";
import ThumbsDownWeightRegular from "../ThumbsDownWeightRegular/ThumbsDownWeightRegular.vue";

defineProps({});
</script>

<template>
  <div class="thumbs">
    <ThumbsUpWeightRegular class="thumbs-up-instance"></ThumbsUpWeightRegular>
    <ThumbsDownWeightRegular
      class="thumbs-down-instance"
    ></ThumbsDownWeightRegular>
  </div>
</template>

<style scoped>
.thumbs,
.thumbs * {
  box-sizing: border-box;
}
.thumbs {
  display: flex;
  flex-direction: row;
  gap: 0.5rem;
  align-items: flex-start;
  justify-content: flex-start;
  position: relative;
}
.thumbs-up-instance {
  flex-shrink: 0 !important;
  width: 1.25rem !important;
  height: 1.25rem !important;
}
.thumbs-down-instance {
  flex-shrink: 0 !important;
  width: 1.25rem !important;
  height: 1.25rem !important;
}
</style>
