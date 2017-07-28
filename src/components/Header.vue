<template>
  <div class="header">
    <img src="../img/arrow.png" class="back" @click="back" height="32" width="32" />
    <span>{{msg}}</span>
  </div>
</template>

<script>
export default {
  name: 'Header',
  props: ['msg'],
  methods: {
    back: function () {
      console.log(11)
    }
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
  .header{
    width: 100%;
    height: 50px;
    position: fixed;
    top: 0;
    left: 0; right: 0;
    background-color: #42b983;
    color: white;
  }
  .header img{
    height: 70%;
    margin-top:5px;
  }
  .header span{
    display: inline-block;
    margin-left: 28%;
    position: relative;
    top: -8px;
  }
</style>
