<template>
  <footer
    v-if="[undefined, 'default', 'auto-col', 'diagram', 'center', 'figure'].includes(this.$slidev.nav.currentLayout)"
    class="absolute bottom-0 right-1 m-2"
  >
    {{ this.$slidev.nav.currentPage }} / {{ this.$slidev.nav.total }}
  </footer>
</template>