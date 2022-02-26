<!-- Please remove this file from your project -->
<template>
  <div class="root">
    <TopBar/>
    <slot/>
  </div>
</template>

<script>
export default {
  name: 'Layout'
}
</script>
<style lang="scss">
@import "../css/common";
</style>
