<template>
	<div class="add">
      <v-header :msg="msg"></v-header>
      <form>
      	<div class="form-item">
      		<label>时间：</label><input type="text" >
      	</div>
        <div class="form-item">
      		<label>时间：</label><input type="text" >
      	</div>      	
        <div class="form-item">
      		<label>时间：</label><input type="text" >
      	</div>      	
      </form>
	</div>
</template>

<script>
import Header from '../components/Header.vue'
export default {
  name: 'add',
  data () {
    return {
      msg: '添加todo'
    }
  },
  components: {
    'v-header': Header
  }
}
</script>

<style>
form{
	margin-top: 50px;
	width: 70%;
	margin-left: 15%;
}
.form-item{
	margin-top: 30px;
}
</style>