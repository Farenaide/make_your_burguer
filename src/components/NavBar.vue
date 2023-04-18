<template>

	<nav>     
		<RouterLink class="logo-burguer" to="/">
			<img :src="logo" :alt="alt" id="logo">
			<h1>Make Your Burguer</h1>
		</RouterLink>   
		<RouterLink to="/"> Home </RouterLink>
		<RouterLink to="/pedidos"> Pedidos </RouterLink>
	</nav>

</template>

<script>

	export default {
		name: 'NavBar',
		props: ["logo", "alt"]
	}

</script>

<style scoped>

	nav{
		background-color: #222;
		border-bottom: 4px solid #111;
		padding: 15px 50px;
		display: flex;
		align-items: center;
		justify-content: flex-end;
		font-size: 30px;
	}

	.logo-burguer{
		box-sizing: border-box;
		margin: auto;
		margin-left: 0;
		display: flex;
		align-items: center;
		background-color: #ffffff25;
		padding: 10px;
		border-radius: 20px;
	}

	nav img{
		width: 50px;
		height: 50px;
	}

	nav a {
		color: #FCBA03;
		text-decoration: none;
		margin: 12px;
		transition: .5s;
	}

	nav a:hover{
		color: #fff;
	}

	h1{
		color: #FCBA03;
		font-family: Verdana, Geneva, Tahoma, sans-serif;
		margin: 0;
		margin-left: 15px;
		font-size: 25px;
	}

</style>