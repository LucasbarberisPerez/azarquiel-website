<script>
    import imgcourse from '../../img/videogame-img/bg.png'
    import {slide} from 'svelte/transition';
    import { onMount } from 'svelte';
  	let ready = false;
  	onMount(() => ready = true);
</script>

{#if ready }     
 
<div class="container-fluid bg-blue-photo" transition:slide="{{ y: -50, duration: 2500, delay: 300 }}">
    
    <div class="container p-2">
        
        <div class="row text-center">
            <div class="col">
                <h2>Curso de especialización de Videojuegos</h2>
            </div>
        </div>

        <div class="row d-flex justify-content-center">
            <img src="{imgcourse}" class="img-fluid" alt="">
       </div>

       <div class="row text-center">
            <div class="col">
                <h3><i class="fa-solid fa-hourglass-half"></i> Duración del curso</h3>
                <p>Total: 600h</p>
                <p>Total horas semanales: 19h</p>
            </div>

            <div class="col">
                <h3>Horario</h3>
                <p><i class="fa-solid fa-moon"></i> Horario vespertino: 15:40 - 21:40</p>
                <p><i class="fa-regular fa-sun"></i> Horario diurno: 8:40 - 14:40</p>
            </div>     
       </div>

      

       <div class="row">
            <div class="col d-flex flex-column justify-content-center border border-1">
                <div class="row"><h3>Contenidos</h3></div>
                
                <div class="row ">
                    <div class="col">
                        <ol> 
                            <li>Diseño de Videojuegos</li>
                                <ul>
                                    <li>
                                        Fundamentos de Computadores
                                    </li>
                                    <li>
                                        Fundamentos de la Programación I y II
                                    </li>
                                    <li>
                                        Matemática Discreta
                                    </li>
            
                                    <li>
                                        Metodologías Ágiles de Producción 
                                    </li>
                                </ul>
                            <li>Desarrollo de Sistemas Interactivos</li>
                                <ul>
                                    <li>
                                        Estructura de Computadores 
                                    </li>
                                    <li>
                                        Estructura de Datos y Algoritmos
                                    </li>
                                    <li>
                                        Informática Gráfica I 
                                    </li>
                                </ul>
                            <li>Diseño de objetos</li>
                                <ul>
                                    <li>
                                        Modelado en 2D y 3D 
                                    </li>
                                    <li>
                                        Programación de Videojuegos en Leguajes Interpretados 
                                    </li>
                                    <li>
                                        Tecnología de la Programación de Videojuegos I y II
                                    </li>
            
                                    <li>
                                        Inteligencia Artificial para Videojuegos
                                    </li>
                                </ul>
            
                            <li>Usabilidad y Análisis de Juegos</li>
                                <ul>
                                    <li>
                                        Desarrollo seguro
                                    </li>
                                    <li>
                                        Videojuegos en Consola
                                    </li>
                                    <li>
                                        Videojuegos para Dispositivos Móviles 
                                    </li>
            
                                    <li>
                                        Testing de Software 
                                    </li>
                                </ul>
                                
                        </ol>
                    </div>
                    
                    
                </div>
                
            </div>
       </div>
        

       


    </div>
    
    
</div>
{/if}
<style lang="sass">
    div.bg-blue-photo
        background: url(../../img/panoramicaAzarquielAzul.jpg)
        background-repeat: no-repeat
        background-size: cover
        background-attachment: scroll
    div
        color: #fff
    h3
        font-size: 1.625rem
        font-weight: bold
    h2
        font-size: 2.625rem
        font-weight: bold
    p
        font-size: 0.875rem
    img
        width: 500px
        height: 350px
        object-fit: cover
        background-repeat: no-repeat
        border-radius: 1.5rem
</style>
