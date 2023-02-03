<script>
	import Navbar from '../components/Navbar.svelte';
	import InfoHeader from '../components/InfoHeader.svelte';
</script>

<div class="container-fluid">
	<header>
		<InfoHeader/>
		<Navbar />
	</header>
	<div class="container">
		<main>
			<slot />
		</main>
	</div>

	<footer>
		<h2>esto es un footer</h2>
	</footer>
</div>

<style lang="sass">
	@import url('https://fonts.googleapis.com/css2?family=Open+Sans:wght@300&display=swap')
	*
		padding: 0
		margin: 0
		font-family: 'Open Sans', sans-serif
		font-weight: 300
</style>
