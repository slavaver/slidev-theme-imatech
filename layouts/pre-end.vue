<template>
  <div class="slidev-layout end">
    <p>Вопросы?</p>
    <p>Комментарии?</p>
    <p>Предложения?</p>
  </div>
</template>

<style scoped lang="postcss">
.slidev-layout.end {
  @apply text-current bg-green-500 h-full text-left grid place-content-center select-none bg-repeat;
  background-image: url(bg-green.png);
  p {
    @apply text-6xl font-500 leading-20;
  }
}
</style>
