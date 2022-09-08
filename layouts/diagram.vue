<template>
  <div class="slidev-layout default">
    <slot />
    <div class="grid h-100 place-content-center">
      <slot name="diagram" />
    </div>
  </div>
</template>
