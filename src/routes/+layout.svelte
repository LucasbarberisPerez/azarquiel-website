<script>
	import Navbar from '../components/Navbar.svelte';
	import InfoHeader from '../components/InfoHeader.svelte';
</script>

<div class="container-fluid">
	<header>
		<InfoHeader/>
		<Navbar />
	</header>
	
		<main>
			<slot />
		</main>

	<footer>
		<h2>Footer</h2>
	</footer>
</div>

<style lang="sass">
	@import url('https://fonts.googleapis.com/css2?family=Open+Sans:wght@300&display=swap')
	*
		margin: 0
		padding: 0
		font-family: 'Open Sans', sans-serif
		font-weight: 300
</style>
