<script>
    import imgcourse from '../../img/cybersecurity-img/bg.webp'
    import {slide} from 'svelte/transition';
    import { onMount } from 'svelte';
  	let ready = false;
  	onMount(() => ready = true);
</script>

<div class="container-fluid bg-blue-photo" transition:slide="{{ y: -50, duration: 2500, delay: 300 }}">
    
    <div class="container p-2">
        
        <div class="row text-center">
            <div class="col">
                <h2>Curso de especialización de Ciberseguridad</h2>
            </div>
        </div>

        <div class="row d-flex justify-content-center">
            <img src="{imgcourse}" class="img-fluid" alt="">
       </div>

       <div class="row text-center">
            <div class="col">
                <h3> <i class="fa-solid fa-hourglass-half"></i> Duración del curso</h3>
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
                            <li>Gobierno de seguridad</li>
                                <ul>
                                    <li>
                                        Arquitecturas de seguridad
                                    </li>
                                    <li>
                                        Introducción y gestión de ciberseguridad
                                    </li>
                                    <li>
                                        Gobierno de ciberseguridad
                                    </li>
            
                                    <li>
                                        Auditoría y control de la seguridad
                                    </li>
                                </ul>
                            <li>Análisis de gestión y riesgos</li>
                                <ul>
                                    <li>
                                        Identificación y gestión de riesgos
                                    </li>
                                    <li>
                                        Análisis y gestion de riesgos y amenazas
                                    </li>
                                    <li>
                                        Riesgos tecnológicos
                                    </li>
                                </ul>
                            <li>Cumplimiento legal y normativo</li>
                                <ul>
                                    <li>
                                        Aspectos legales y regulatorios asociados a Privacida
                                    </li>
                                    <li>
                                        Técnicas, metodologías y herrramientas del compliance legal
                                    </li>
                                    <li>
                                        Notificación, reporte, denuncia y presentación en juzgado
                                    </li>
            
                                    <li>
                                        Cibercrimen y delitos informátivos
                                    </li>
                                </ul>
            
                            <li>Operativa de ciberseguridad</li>
                                <ul>
                                    <li>
                                        Desarrollo seguro
                                    </li>
                                    <li>
                                        Criptografía
                                    </li>
                                    <li>
                                        Monitorización de seguridad
                                    </li>
            
                                    <li>
                                        Análisis de vulnerabilidades
                                    </li>
                                </ul>
                                
                            <li>Ciber inteligencia, cooperacion y capacidad</li>
                            <ul>
                                <li>
                                    Relaciones con organismos nacionales e Internacionales
                                </li>
                                <li>
                                    Ciber Ejercicios
                                </li>
                                <li>
                                    Intercambio de información con terceros e IoCs
                                </li>
            
                                <li>
                                    Gestión y respuesta a incidentes de Seguridad
                                </li>
                            </ul>
                        </ol>
                    </div>
                    
                    
                </div>
                
            </div>
       </div>
        

       


    </div>
    
    
</div>

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
        height: 200px
        object-fit: cover
        background-repeat: no-repeat
        border-radius: 1.5rem
</style>
