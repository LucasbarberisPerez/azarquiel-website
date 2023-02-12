<script>
    import imagenCiberseguridad from '../../img/home-img/ciberseguridad-card.jpg'
    import imagenVideojuegos from '../../img/home-img/videojuegos-card.webp'
</script>
<div class="container mb-4">
    <div class="row">
        <h2 class="text-center">Novedades</h2>
        <h3>Nuevos cursos de especialización</h3>
    </div>
    <div class="row">
        <div class="col">
            <div class="card text-center h-100">
              <img class="card-img-top" src="{imagenCiberseguridad}" alt="Title">
              <div class="card-body d-flex flex-column justify-content-center align-items-center">
                <h4 class="card-title">Curso completo de Hacking Ético y Ciberseguridad</h4>
                <p class="card-text">Aprende Hacking Ético y Ciberseguridad de manera práctica, ¡conviértete en un experto en Hacking Ético y Ciberseguridad!</p>
                <a href="/cybersecurity">Ver más</a>
              </div>
            </div>
        </div>

        <div class="col">
            <div class="card text-center h-100">
              <img class="card-img-top" src="{imagenVideojuegos}" alt="Title">
              <div class="card-body card-body d-flex flex-column justify-content-center align-items-center">
                <h4 class="card-title">Curso de diseño y desarrollo de videojuegos</h4>
                <p class="card-text">Conviertete en el mejor artista digital de Videojuegos estudiando con los mejores profesionales del sector y en la escuela de referencia a nivel provincial.</p>
                <a href="/videogame">Ver más</a>
              </div>
            </div>
        </div>
    </div>

</div>

<style lang="sass">
    img
        object-fit: cover
        height: 350px
    a
        max-width: 300px
        width: 250px
        padding: 0.5rem
        background-color: #1E90FF
        color: #fff
        text-align: center
        border: 1px black solid
        border-radius: 1.5rem
        text-decoration: none
        font-weight: bold
        transition: all 0.15s ease-in-out
        &:hover
            cursor: pointer
            background-color: #00BFFF
        
        
</style>