<script setup>
	import { RouterView } from 'vue-router'
</script>

<template>
	<NavBar :logo="logo_src" :alt="app_name" />
	<RouterView />
	<MainFooter/>
</template>

<script>

	import NavBar from './components/NavBar.vue';
	import MainFooter from './components/MainFooter.vue';

	export default{
		components:{
		NavBar,
		MainFooter
	},
	data(){
		return{
		logo_src: "/img/logo.png",
		app_name: 'Make Your Burguer Logo'
		}
	}
	}

</script>

<style>
	body{
		font-family: Arial, Helvetica, sans-serif;
		min-height: 100vh;
	}

	#app{
		display: flex;
		flex-direction: column;
		min-height: 100vh;
	}

	.main-container{
		margin: 50px;
		min-height: 250px;
	}

	h1{
		text-align: center;
		font-size: 42px;
		margin-bottom: 30px;
		color: #222;
	}

</style>
