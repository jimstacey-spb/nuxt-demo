<template>
  <div class="topbar">
    <nuxt-link :to="localePath('/')"><img src="../images/logo.svg" alt="Logo"/></nuxt-link>
    <div class="topbar__language-change">
      <img src="../images/en-flag.svg" lang='en' alt="" @click="$i18n.setLocale('en')"/>
      <img src="../images/ru-flag.svg" lang='ru' alt="" @click="$i18n.setLocale('ru')"/>
    </div>
    <TopBarMenu/>
  </div>
</template>

<script>
export default {
  name: 'TopBar'
}
</script>

<style lang="scss">
@import "../css/topbar";
</style>
