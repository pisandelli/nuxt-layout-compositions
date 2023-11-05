<script lang='ts' setup>
/**
* One Header-Body-Footer (HBF)
* layout to rule them all
* @name 'BasicLayout'
* @version 1.0.1
*/
</script>

<template>
<div class='hbf-layout'>
  <slot />
</div>
</template>

<style scoped>
.hbf-layout {
  display: grid;
  grid-template-rows: min-content auto min-content;
  gap: var(--lc-gap, 1.5rem) 0;
  min-block-size: 100vh;
}
</style>
