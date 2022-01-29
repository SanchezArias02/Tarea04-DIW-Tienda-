<template>
  <footer id="pie">
    <div class="flx">
      <!-- <div class="grow"></div> -->
      <div class="conocenos"> 
         <div class="descrip">
           <h3>Nuestra empresa</h3>
              <nav>
                <ul>
                  <li><a href="#">¿Quienes somos?</a></li>
                  <li><a href="#">Seguridad informática</a></li>
                  <li><a href="#">Colaborador Inse-Techter</a></li>
                  <li><a href="#">Futuros proyectos</a></li>
                  <li><a href="#">Compromiso medioambiental</a></li>
                </ul>
              </nav>
         </div>
         <div class="red_social">
            <h3>Contactos</h3>
              <nav>
                <ul>
                  <li><a href="#">Atención telefónica</a></li>
                  <li><a href="#">Formulario de contacto</a></li>
                </ul>
              </nav>
              <img src="../assets/Iconos-img/redes-sociales.png" alt="Redes sociales" copyright="cc-by Redes sociales"/>

         </div>
      </div>
      <div class="izq">
          <div class="asociados">
            <h3>Asociados</h3>
              <nav>
                <ul>
                  <li><a href="https://cifpcarlos3.es/"><img src="../assets/Logotipos/cifp.png" alt="Cifp carlosIII" copyright="cc-by-sa Cifp Carlos III"></a></li>
                  <li><a href="#"><img src="../assets/Logotipos/vue.png" alt="vue.js" copyright="cc-by-sa Vue.js"></a></li>
                </ul>
              </nav>
          </div>
          <div class="colaboradores">
            <h3>Colaboradores</h3>
              <nav>
                <ul>
                  <li><a href="#">Empresas nacionales</a></li>
                  <li><a href="#">Empresas internacionales</a></li>
                </ul>
              </nav>
          </div>
      </div>
      <div class="der">
        <div class="der-arriba">
          <h3>Garantía Inse-Tech</h3>
          <img src="../assets/Logotipos/confianza-online.png" alt="Confianza online" copyright="cc-by-sa Confianza online">
          <img src="../assets/Logotipos/com_eur.png" alt="Adigital" copyright="cc-by-sa Comision Europea">
          <img src="../assets/Logotipos/adigital_logo.png" alt="Comision Europea" copyright="cc-by-sa Adigital">
        </div>
        <div class="der-centro">
          <h3>Métodos de Pago</h3>  
          <img src="../assets/Logotipos/metodos-pago.png" alt="Metodos de pago" copyright="cc-by-sa Metodos pago"/>
        </div>
        <div class="der-abajo"></div>
        <h3>Socios mensajeros</h3>
          <div class="contenedor">
            <img src="../assets/Logotipos/dhl.png" alt="DHL" copyright="cc-by-sa DHL">
            <img src="../assets/Logotipos/fedex.png" alt="Fedex" copyright="cc-by-sa Fedex"/>
            <img src="../assets/Logotipos/españa.png" alt="Correos" copyright="cc-by-sa Correos"/>
          </div>
      </div>
    </div>
    <p><span id="cookies"><a href="#">Avisos Legales</a></span>© Copyright 2022 - Todos los derechos reservados <span id="cookies"><a href="#">COOKIES</a></span></p>
  </footer>
</template>

<script>
export default {
}
</script>

<style scoped>

/* General */

footer#pie {
    background-color: #ebebeb;
}
#pie p {
    color: rgb(0, 0, 0);
    text-align: center;
    font-size: 12px;
    position: relative;
}

.flx{
  display:flex;
  justify-content: space-around;
  
}

div > nav ul{
  list-style: none;
}

div > nav ul li a{
  text-decoration: none;
  color:#63717f;
  font-size: 14px;
}

.grow{
  flex-grow: 1;
}

/* Cookies */

span#cookies{
  margin: 0 2em 0 2em;
  font-weight: 600;
}

span#cookies:hover{
  text-decoration: underline;
}

span#cookies > a{
  text-decoration: none;
  color: black;
}

/* Izquierda */
  .izq{
   padding: 3em;  
}

  .izq .asociados img{ 
  height: 70px;
}


/* Centro */

.conocenos{
  /* background-color: white; */
  margin: 0 0 0 7em;
  padding: 3em;
  background-color: rgb(255, 255, 255);
  border-bottom-left-radius: 150px;
  border-bottom-right-radius: 150px;
}

.red_social{
  align-items:center;
  justify-content: center;
}

.red_social > img{ 
  height: 80px;
  margin: 0 2em 0 2em;
}


/* Derecha */

.der{
  padding: 3em;
}

.der-arriba > img{
  height: 40px;
  /* padding: 0 0.5em 0 0; */
}

.der-centro > img{
  height: 30px;
  /* margin: 1em 3em 2em 0; */
}
 .contenedor > img{
  height: 45px;
  background-color: white;
  margin: 0 0.5em 0 0;
}
</style>