<template>
  <Layout>
    <div class="contests-page">
      <h1>{{ $t('contests_page.title') }}</h1>
      <div class="contests-page__cover-list">
        <nuxt-link class="contests-page__cover" to="/contests/africa">
          <img src="../../images/africa-contest.jpg" alt=""/>
          {{ $t('contests_page.africa') }}
        </nuxt-link>

        <nuxt-link class="contests-page__cover" to="/contests/india">
          <img src="../../images/india-contest.jpg" alt=""/>
          {{ $t('contests_page.india') }}
        </nuxt-link>
      </div>
    </div>
  </Layout>
</template>

<style lang="scss">
  @import "css/contests";
</style>
