<template>
  <Layout>
    <h1 class="main-page__title">{{ $t('html_title') }}</h1>
    <div class="main-page__flag">
      <img :src=flagPath alt=""/>
    </div>
  </Layout>
</template>

<script>
export default {
  computed: {
    flagPath() {
      return require(`../images/${this.$i18n.locale}-flag.svg`);
    }
  }
}
</script>
<style lang="scss">
  @import '../css/main-page.scss';
</style>
