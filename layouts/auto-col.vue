<script setup>
import { computed } from "vue";
const props = defineProps({
  colNumber: {
    type: Number,
  },
});
const cols = computed(() => {
  const colNames = [];
  for (let i = 1; i <= props.colNumber; i++) {
    colNames.push(`autoCol${i}`);
  }
  return colNames;
});
</script>

<template>
  <div class="slidev-layout default auto_cols">
    <slot />
    <div class="grid gap-4 grid-rows-1 min-h-3/5" :class="`grid-cols-${props.colNumber}`">
      <div v-for="col in cols">
        <slot :name="col" />
      </div>
    </div>
    <slot name="footer" />
  </div>
</template>

<style scoped lang="postcss"></style>
