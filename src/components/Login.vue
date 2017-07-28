<template>
	<div class="login_main">
		<v-header :msg="msg"></v-header>
		<img src="../img/headPicture.jpg" class="logo" /><br />
		<input type="text" /><br />
		<button><router-link to="home">登录</router-link></button>
	</div>
</template>

<script>
import Header from '../components/Header.vue'
export default {
  name: 'login',
  data () {
    return {
      msg: '登录'
    }
  },
  components: {
    'v-header': Header
  }
}
</script>

<style>
	.logo,input,button{
		display: block;
		margin: 20px auto;
		width: 50%;
	}
	.logo{
		margin-top: 100px;
	}
	input{
		height: 50px;
	}
	button{
		height: 50px;
		background-color: orange;
		color: white;
		border: none;
	}
</style>