<template>
  <div class="grid grid-cols-2 w-full h-full">
    <div
      class="slidev-layout default plan text-left left-side text-white grid items-center"
    >
      <slot />
    </div>
    <div class="slidev-layout default plan grid items-center">
      <slot name="plan" />
    </div>
  </div>
</template>

<style scoped lang="postcss">
.left-side {
  @apply bg-repeat;
  background-image: url(bg-orange.png);
}
</style>
