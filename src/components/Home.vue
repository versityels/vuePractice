<template>
  <div class="main">
    <v-header :msg="msg"></v-header>
    <div class="content">
      <button><router-link to="/home/addTodo">添加todo</router-link></button>

      <button><router-link to="/home/todoList">todo列表</router-link></button>
    </div>
  </div>
</template>

<script>
  import Header from '../components/Header.vue'
  export default {
    name: 'home',
    data () {
      return {
        msg: '用户中心'
      }
    },
    components: {
      'v-header': Header
    }
  }
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style>
.content{
  margin-top: 50px;
}
.content button{
  width: 70%;
  height: 50px;
  background-color: orange;
  color: white;
  margin: 30px 15%;
  border: none;
  border-radius: 5px;
}
</style>
