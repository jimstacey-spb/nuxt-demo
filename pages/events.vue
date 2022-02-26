<template>
  <Layout>
    <div class="events-page__intro">
      <h4>
        {{$t('events_page.dogs_dialog')}}
      </h4>
    </div>
    <div class="wrapper">
      <div class="events-page__photos">
        <img v-for="image in dogs" :src="image" alt="" :key="image"/>
      </div>
    </div>
  </Layout>
</template>

<script>
export default {
  data() {
    return {
      dogs: []
    }
  },
  async fetch() {
    this.dogs = await fetch('https://dog.ceo/api/breed/pomeranian/images/random/20')
      .then(res => res.json())
      .then(result => result.message);
  }
}
</script>

<style lang="scss">
  @import "../css/events-page";
</style>
