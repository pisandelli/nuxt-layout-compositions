<script lang='ts' setup>
/**
* One Header-Body-Footer (HBF)
* layout to rule them all
* @name 'BasicLayout'
* @version 1.0.0
*/
</script>

<template>
<div class='hbf-layout'>
  <header>
    <slot name='header' />
  </header>
  <main>
    <slot />
  </main>
  <footer>
    <slot name='footer' />
  </footer>
</div>
</template>

<style lang="stylus" scoped>
.hbf-layout
  display: grid
  grid-template-rows: var(--lc-header-height, min-content) auto var(--lc-footer-height, min-content)
  gap: var(--lc-gap, 1.5rem) 0
  min-block-size: 100vh
</style>
