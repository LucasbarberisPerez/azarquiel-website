<script>
	import { Router, Link, Route } from 'svelte-routing';
	import Login from '../routes/ciberseguridad.svelte';
    import imagen from '../img/logoiesfseif.png'
</script>

<h1>Navegación</h1>
<Router>
	<div class="top-menu">
		<nav>
            <Link to="/"><img src={imagen} alt="Imagen"></Link>
            
			<Link to="/">Inicio</Link>
			<Link to="/login">Videojuegos</Link>
			<Link to="/perfil">ciberseguridad</Link>
		</nav>
	</div>

	<Route path="/" />
	<Route path="/login">
		<Login />
	</Route>
	<Route path="/perfil" />
</Router>

<style>
    @import url('https://fonts.googleapis.com/css2?family=Open+Sans:wght@300&display=swap');
    div.top-menu{
        width: 100%;
        font-family: 'Franklin Gothic Medium', 'Arial Narrow', Arial, sans-serif;

        border: 1px black solid;
    }
	nav {
		display: flex;
		flex-direction: row;
		gap: 1.5rem;
		font-size: larger;
		font-family: 'Open Sans', sans-serif;
        font-weight: 100;
		font-weight: bold;
		justify-content: left;
		align-items: center;
        text-decoration: none;
        
	}
</style>
