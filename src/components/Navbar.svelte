<script>
	import imagen from '../img/logoiesfseif.png';
</script>

<nav class="navbar navbar-expand-lg sticky-top">
	<div class="container-fluid">
		<a class="navbar-brand ms-5" href="/"><img src={imagen} alt="" class="img-logo" /></a>
		<button
			class="navbar-toggler toggle-button"
			type="button"
			data-bs-toggle="collapse"
			data-bs-target="#navbarScroll"
			aria-controls="navbarScroll"
			aria-expanded="false"
			aria-label="Toggle navigation"
		>
		
		<i class="fa-solid fa-bars"></i>
		</button>
		<div class="collapse navbar-collapse text-end" id="navbarScroll">
			<ul
				class="navbar-nav ms-auto my-2 my-lg-1 navbar-nav-scroll"
				style="--bs-scroll-height: 100%; --bs-scroll-width:200px;"
			>
				<li class="nav-item">
					<a class="nav-link" aria-current="page" href="/">inicio</a>
				</li>
				<li class="nav-item">
					<a class="nav-link" href="/">al día</a>
				</li>

				<li class="nav-item">
					<a class="nav-link" href="/">el loro</a>
				</li>
				<li class="nav-item">
					<a class="nav-link" href="/">el centro</a>
				</li>

				<li class="nav-item">
					<a class="nav-link" href="/">secretaría</a>
				</li>

				<li class="nav-item">
					<a class="nav-link" href="/">familias</a>
				</li>

				<li class="nav-item">
					<a class="nav-link" href="/">bolsa</a>
				</li>
			</ul>
		</div>
	</div>
</nav>

<style lang="sass">
	//<span class="navbar-toggler-icon toggle-span" />
	img.img-logo
		max-width: 250px
		max-height: 250px
	nav
		background: #ffffff
		font-size: 0.8rem
	i
		color: black
	button
		border: none
	a
		color: #000
		&:active
			color: #22B8F0
</style>
