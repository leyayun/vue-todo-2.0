<style>
body {
  font-family: Helvetica, sans-serif;
  margin: 0;
}

</style>

<template>
  <div id="app">
    <pager-header></pager-header>
    <h1>{{ msg }}</h1>
  </div>
</template>

<script>
import PagerHeader from './PagerHeader.vue'

export default {
  components: {
    'pager-header':  PagerHeader
  },
  data () {
    return {
      msg: 'TODO'
    }
  }
}
</script>

