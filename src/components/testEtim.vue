<template>
	<button @click="testEtim">testEtim</button>
</template>

<script>
export default {
	data(){
		return{
			
		}
	},
	methods:{
		testEtim(){
			alert(this.$route.query.id);
		}
	}
}
</script>

<style>
</style>