<style scoped>
  header {
    color: white;
    font-size: 18px;
    background: #000;
    line-height: 44px;
    text-align: center;
  }
</style>

<template>
  <div>
    <header>{{title}}</header>
  </div>
</template>

<script>
  export default {
    data(){
      return {
        title: "A simple todo demo build with vue-2.0"
      }
    }
  }
</script>