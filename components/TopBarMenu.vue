<template>
  <div class="topbar__menu">
    <nuxt-link v-for="item in menuItems" class="topbar__menu-item" :to="item.url" :data-test="item.dataTest" :key="item.url">{{$t(item.i18nKey)}}</nuxt-link>
  </div>
</template>

<script>
export default {
  data() {
    return {
      menuItems: [
        {
          url: '/',
          i18nKey: 'about',
          dataTest: "menu_about"
        },
        {
          url: '/contests',
          i18nKey: 'contests',
          dataTest: "menu_ibs_long"
        },
        {
          url: '/events',
          i18nKey: 'events',
          dataTest: "menu_contests"
        },
      ]
    }
  }
}
</script>
