<script>

	export default{
		data: () => ({
			contador: 100
		}),
		methods: {
			sumar() {
				this.contador++;
			},
			restar() {
				this.contador--;
			},
			resetear() {
				this.contador = 100;
			}
		}

	}

</script>

<template>
  <div class="container">

	<img src="./assets/logo.svg" alt="Logo" width="125" height="125">
	<h1>Hola mundo desde Vue js</h1>
	<link rel="stylesheet" href="../public/base.css">

	<h2>Contador: {{ contador }}</h2>
	<button @click="sumar">+1</button>
	<button @click="restar">-1</button>
	<button @click="resetear">Reset</button>

  </div>

</template>

<style scoped>

.container{
  	text-align: center;
}

h1{
	font-weight: bolder;
	color: gray;
}

h2{
	font-size: 2.5rem;
}

button{
	font-size: 1.5rem;
	margin: 0px 10px;
	cursor: pointer;
}

</style>