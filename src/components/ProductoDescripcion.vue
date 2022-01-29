<template>
 <section id="producto-descripcion">
     <div class="indice">
         <div class="indice-desc">
             <a href="#descripcion"><img src="../assets/Iconos-svg/flecha.svg" alt="flecha indice" copyright="cc-by-sa Google Icons"/> Descripción</a>
         </div>
         <div class="indice-caract">
              <a href="#caracteristicas"><img src="../assets/Iconos-svg/flecha.svg" alt="flecha indice" copyright="cc-by-sa Google Icons"/> Caracteristicas técnicas</a>
         </div>
         <div class="indice-opi">
             <a href="#opiniones"><img src="../assets/Iconos-svg/flecha.svg" alt="flecha indice" copyright="cc-by-sa Google Icons"/> Tecnología de punta</a>
         </div>
    </div>
    
    <div id="total-descripcion">
        <div class="container">
            <div class="texto">
                <h3 id="descripcion">Descripción</h3>
                <ul>
                    <li>Pantalla grande, portátil pequeño.</li>
                    <li>Potencia para cada movimiento. Este portátil gaming cuenta con un potente procesador Intel y gráficos NVIDIA, que podrán con todo lo que les eches. El sistema térmico mejorado mantiene el equipo a una temperatura más fresca para que puedas jugar con más intensidad, mejor, más rápido y más tiempo.</li>
                    <li>Diseñado pensando en el jugador. Conéctate desde donde quieras gracias al Wi-Fi con velocidades Gigabit. El SSD PCIe de gran capacidad te permite guardar archivos más rápido que nunca. Además, incluye una amplia variedad de puertos de E/S para que puedas conectar todos los accesorios que quieras.</li>
                    <li>Seguridad total. Hoy en día utilizamos los dispositivos electrónicos para todo tipo de cosas; desde transacciones bancarias hasta el almacenamiento de documentos importantes. Por ello, la seguridad nunca está de más. El portátil HP cuenta con la más óptima tecnologia en seguridad Wolf Security </li>
                </ul>
            </div>
           
            <div class="texto">
                 <h3 id="caracteristicas">Caracteristicas técnicas</h3>
                    <ul>
                        <li>Windows 11 Home </li>
                        <li>Intel® Core™ i5-1155G7 (hasta 4,5 GHz con tecnología Intel® Turbo Boost, 8 MB de caché L3, 4 núcleos, 8 subprocesos)</li>
                        <li>RAM DDR4-3200 MHz 8 GB (2 x 4 GB)</li>
                        <li>FHD de 14" (35,6 cm) en diagonal, IPS, bisel micro-edge, antirreflectante, 250 nits, 45 % NTSC (1920 x 1080) </li>
                        <li>Gráficos Intel® Iris® Xᵉ</li>
                        <li>HP Wolf Security</li>
                    </ul>
            </div>

            <div class="texto">
                <h3 id="opiniones">Tecnología de punta</h3>
                <h5>HP Wolf Security</h5>
                <p><strong>"</strong>En vez de intentar reconocer las amenazas, lo que puede resultar problemático si alguna consigue “camuflar” 
                    sus malas intenciones, lo que hace <b>es crear una máquina virtual 
                    totalmente aislada del sistema anfitrión</b>, y es dentro de la misma donde abre dicho archivo o web.<strong>"</strong>&nbsp; - &nbsp;<strong> muyseguridad.net</strong></p>
                <div class="videos">
                    <iframe width="450" height="250" src="https://www.youtube.com/embed/G_ECagEVZAY" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                    <video controls>
                        <source src="../assets/Media/Publicidad_HP.mp4" type="video/mp4">
                    </video>
                </div>
            </div>
        </div>
    </div>
  </section>
    
</template>

<script>

</script>

<style scoped>

@import url('https://fonts.googleapis.com/css2?family=Montserrat:ital@1&display=swap');

/*Icono arrow*/

@import url('https://fonts.googleapis.com/css?family=Material+Icons+Outlined');

/* General */
#producto-descripcion {
    margin:2rem;
}
#producto-descripcion h2 {
    color: #101010;
}

div#total-descripcion{
    display:inline-block;
}

.container > *{
    margin: auto;
    max-width: 60%;
    
}

/* Barra indice contenido */

.indice{
    display:flex;
    justify-content:space-around;
    border-top:1px solid rgb(235, 232, 232);
    box-shadow: 0px 2px 4px #999;
    height:50px;
    align-items:center;
}

.indice a{
    text-decoration: none;
    color: #101010;
    font-size: 18px;
}

.indice a img{
    height:16px;
}


/* Texto */

.texto p{
  font-family: 'Montserrat', sans-serif;  
  margin:1em;
}

.texto > iframe{
    justify-content: center;
    align-items: center;
}

/* Videos */

.videos{
    display: flex;
}

.videos > video{
    width: 450px;
    margin: 1em;
}

iframe{
    margin: 1em;
}
</style>
