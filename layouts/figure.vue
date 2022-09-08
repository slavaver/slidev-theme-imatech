<script setup lang="ts">
const props = defineProps({
  imgUrl: {
    type: String,
  },
});
</script>

<template>
    <figure class="slidev-layout">
      <img :src="props.imgUrl" alt="props.caption" />
      <figcaption><slot /></figcaption>
    </figure>
</template>

<style scoped lang="postcss">
figure {
  @apply w-full h-11/12 p-4;
}
img {
  @apply w-auto h-auto max-w-full max-h-full object-center object-contain mx-auto rounded-xl;
}

figcaption {
  @apply mt-4 text-center;
}
</style>
