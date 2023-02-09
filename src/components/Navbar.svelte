<script>
	import { page } from '$app/stores';
	import imagen from '../img/logoiesfseif.png';
	const navlinks = [
		{ title: 'home', href: '/' },
		{ title: 'al día', href: '#' },
		{ title: 'el loro', href: '#' },
		{ title: 'el centro', href: '#' },
		{ title: 'secretaría', href: '#' },
		{ title: 'familias', href: '#' },
		{ title: 'bolsa', href: '#' }
	];
	$: current = $page.route.id;
</script>

<div class="container">
	<div class="row">
		<nav class="navbar  navbar-expand-lg">
			<a class="navbar-brand ms-5" href="/"><img src={imagen} alt="" class="img-logo" /></a>
			<button
				class="navbar-toggler toggle-button shadow-none"
				type="button"
				data-bs-toggle="offcanvas"
				data-bs-target="#offcanvas"
				aria-controls="offcanvas"
				aria-expanded="false"
				aria-label="Toggle navigation"
			>
				<i class="fa-solid fa-bars" />
			</button>
			<div class="collapse navbar-collapse">
				<ul class="navbar-nav ms-auto my-2 my-lg-1">
					{#each navlinks as { title, href }}
						<li class="nav-item">
							<a
								class={current == href ? 'nav-link active-link' : 'nav-link'}
								aria-current="page"
								href={href}>{title}</a
							>
						</li>
					{/each}
				</ul>
			</div>
		</nav>

		<!--Navegador lateral-->
		<div class="offcanvas offcanvas-end end-menu" tabindex="-1" id="offcanvas" aria-labelledby="offcanvasLabel">
			<!--Aqui comienza el header-->
			<div class="offcanvas-header">
				<h5 class="offcanvas-title" id="offcanvasScrollingLabel">Menú lateral</h5>
				
				<button
					class="btn-close btn-close-white text-reset shadow-none"
					data-bs-dismiss="offcanvas"
				/>
			</div>
			<!--Aquí comienza el body-->
			<div class="offcanvas-body" id="lateral-menu">
				<div class="row gap-3">

				
				{#each navlinks as { title, href }}
						<div class="row border-bottom border-bottom-2">
							<a
								class={current == href ? 'nav-link active-link' : 'nav-link'}
								aria-current="page"
								href={href}>> {title}</a
							>
						</div>
							
						
				{/each}
				</div>
			</div>
			
		</div>
	</div>
</div>

<style lang="sass">
	img.img-logo
		max-width: 250px
		max-height: 250px
	nav
		background: #ffffff
		font-size: 0.8rem
	i
		color: black
		&:hover
			color:#22B8F0
	button
		border: none
		text-decoration: none
	a
		color: #000f
		transition: 0.5s all ease-in-out
		&:hover
			color: #22B8F0
	.active-link
		color: #22B8F0
	.end-menu
		background: #333
		color: #ffffff
	#lateral-menu
		text-transform: uppercase
		a
			color: #ffffff
			transition: 0.5s all ease-in-out
			text-decoration: none
			&:hover
				color: #22B8F0
	#offcanvas
		transition: 0.5s all ease-in-out
</style>
