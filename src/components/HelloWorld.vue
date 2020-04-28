<template>
	<div>
  <button class="testRouter" @click="testRouter">测试路由跳转</button>
  <div class="divSty" :is="testIs"></div>
  </div>
</template>

<script>
import testIs from './testIs';
export default {
  data () {
    return {
				testIs:'testIs'
    }
  },
  methods:{
  	testRouter(){
  		//this.$router.push('home');
  		//this.$router.push({path:'login?url'+1});
  		this.$router.push({path:'/test/test',query:{id:'1'}});
  	}
  },
  components:{
  	testIs
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.divSty{
	height: 300px;
	width: 500px;
	border: 2px solid green;
	margin: auto;
}
</style>
