<template>
    <section id ="datos">
        <div class="precio">
            <div class="flx">
                <h2>Portátil Gaming HP Pavilion 16-a0002ns</h2>
                <span>789.-<span>€</span></span><a href="#"><br>Iva incl. / con envío gratis</a><br>
                    <div class="wrapper">
                        <button class="btn" @click="cambiarContador('-1')" type="button" name="button">-</button>
                        <input class="cantidad" type="text" name="name" :value="contador">
                        <button class="btn" @click="cambiarContador('1')" type="button" name="button">+</button>
                    </div><br>
                <div class="botones">
                    <button type="submit">AÑADIR AL CARRITO</button><a class="megusta" href="#" ><img src="../assets/Iconos-img/amor.png" alt="Favorito" copyright="cc-by Icono corazon" height="20" width="20"></a>
                </div>
            </div>
        </div>

        <section id="flex">
            <div class="anhadir">
                <h3>Protecciones</h3>
                <div class="proteccionservicios">
                    <div class="checkboxes">
                        <input type="checkbox">
                    </div>
                    <div class="esc-checkbox">
                        Garantia ampliable +2 años<span class="pago-unico">+99,90€<br>único pago</span>
                    </div>
                </div>
                <div class="proteccionservicios">
                    <div class="checkboxes">
                        <input type="checkbox">
                    </div>
                    <div class="esc-checkbox">
                        Protección avanzada 4 años<span class="pago-unico">+129,80€<br>único pago</span>
                    </div>
                </div>
                <h3>Otros servicios</h3>
                <div class="proteccionservicios">
                    <div class="checkboxes">
                        <input type="checkbox">
                    </div>
                    <div class="esc-checkbox">
                        Cristal templado de Alt/Cal.<span class="pago-unico">+28,99€<br>único pago</span>
                    </div>
                </div>
            </div>
        </section>

    </section>
    
</template>

<script>
export default {
  Name: 'ProductoDatos',
    data () {
        return {
            contador: 1
        }
    },
    methods: {
        cambiarContador(num) {
            this.contador += +num;
            if (!isNaN(this.contador) && (this.contador < 0)) {
              this.contador = 0
            }
        }
    }
}

</script>

<style scoped>

@import url('https://fonts.googleapis.com/css2?family=Bungee+Inline&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@1,300&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Dongle:wght@400;700&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Acme&display=swap');

/*Parte Superior */

section#datos .precio {
    padding-top: 1em;
    align-items:center;
    
}

section#datos .precio{
    border-bottom: 1px solid rgb(199, 198, 198);
    margin: 1em;

}

.precio .flx > span{
    font-family: 'Acme', sans-serif;
    font-weight: 900;
    font-size: 45px;
}

.precio .flx > span > span{
    font-size: 30px;
    margin: 0 0 0 0.5em;
}

.flx span{
    line-height: 1em;
}

.flx > a{
    font-family: 'Montserrat', sans-serif;
    color:grey;
    text-decoration: none;
    font-size: 14px;
}


.flx a:hover{
    text-decoration: underline;
}

.botones{
    display: flex;
}

.botones button{
    background: rgb(250, 249, 249);
    color: rgb(0, 0, 0);
    border-radius: 2px;
    width: 350px;
    height: 36px;
    border: 2px solid rgb(0, 0, 0);
    font-weight: 900;
    margin: 0 0 2em 0;

}

.botones button:hover{
    background: rgb(234, 228, 235);
    padding: 0.3em;
}

.botones a img{
    background: rgb(190, 192, 190);
    border-radius: 2px;
    padding: 0.5em;
    margin: 0 0 0 0.3em;
}

.botones a img:hover{
    background: rgb(164, 165, 164);
}

/*Parte Inferior*/

.anhadir{
    width: 400px;
    margin: 0 0 0 1em;
}

.pago-unico{
    line-height: 1em;
    margin:0 0 0 3em;
    color:black;
    font-weight: bold;
    position: absolute;
    font-size: 14px
}

.anhadir .proteccionservicios{
    font-family: 'Montserrat', sans-serif;
    font-size: 15px;  
    display: flex;
    margin: 1em;
    align-items:center;
}

.proteccionservicios input[type="checkbox"]{
   margin: 0.6em;
}

#flex{
    display:flex;
    align-items:center;
}


/*Contador*/

.wrapper {
  height: 2rem;
  display: flex;
  margin: 1em 0 0 0;
}

.wrapper button:focus, input:focus {
  outline: 0;
}

.cantidad {
  border: none;
  text-align: center;
  width: 2rem;
  font-size: 1.2rem;
  border: 1px solid #d8d8d8;
}

.btn {
  border: 1px solid #d8d8d8;
  width: 1.8rem;
}
</style>
