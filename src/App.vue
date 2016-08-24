<template>
  <div id="app">
    <pager-header></pager-header>
    <div id="content">
      <h1>{{ msg }}</h1>
      <h1 :class="{active: isActive}" @click="active">{{ reversedMsg }}</h1>
      <input type="text" v-model="msg">
    </div>
  </div>
</template>

<style scoped>
  #content {
    padding: 10px 20px;
  }

  .active {
    color: red;
  }
</style>

<script>
import PagerHeader from './components/PagerHeader.vue'

export default {
  components: {
    PagerHeader
  },
  data () {
    return {
      msg: 'TODO',
      isActive: false
    }
  },
  computed: {
    reversedMsg (){
      return this.msg.split('').reverse().join('');
    }
  },
  methods: {
    active(){
      this.isActive = !this.isActive;
    }
  }
}
</script>