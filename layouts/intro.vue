<script setup lang="ts">
const props = defineProps({
  introName: {
    type: String,
  },
  introDate: {
    type: String,
  },
  introTitle: {
    type: String,
  },
  introSubtitle: {
    type: String,
  },
});
</script>

<template>
  <div class="slidev-layout intro">
    <div class="my-auto">
      <h1>{{ props.introTitle }}</h1>
      <h2>{{ props.introSubtitle }}</h2>
      <div class="absolute bottom-20">
        <span class="font-normal">
          {{ props.introName }} / {{ props.introDate }}
        </span>
      </div>
    </div>
  </div>
</template>

<style scoped lang="postcss">
.slidev-layout.intro {
  border-bottom: 5px solid #f05642;
  border-left: 5px solid #25b39e;
  h1 {
    @apply text-6xl leading-20 text-transparent bg-clip-text;
    background-image: linear-gradient(90deg, #f05642 0%, #F88637 100%);
  }

  h2 {
    @apply text-4xl text-transparent bg-clip-text;
    background-image: linear-gradient(90deg, #25b39e 0%, #1b7f70 100%);
  }
}
</style>
