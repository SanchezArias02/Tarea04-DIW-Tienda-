<template>
    <section id="Productos">
       
            <div class="principal">
                <img v-bind:src="fotos[0]" alt="Portátil HP Pavilion 16-a">
            </div>

            <div class="miniatura">
                <a @click='cambiofoto(1)'><img  v-bind:src='fotos[1]' alt="Portátil HP Pavilion 16-a" copyright="cc-by-sa HP"/></a>
                <a @click="cambiofoto(2)"><img  v-bind:src="fotos[2]" alt="Portátil HP Pavilion 16-a" copyright="cc-by-sa HP"/></a>
                <a @click="cambiofoto(3)"><img  v-bind:src="fotos[3]" alt="Portátil HP Pavilion 16-a" copyright="cc-by-sa HP"/></a>
                <a @click="cambiofoto(4)"><img  v-bind:src="fotos[4]" alt="Portátil HP Pavilion 16-a" copyright="cc-by-sa HP"/></a>
            </div>

    </section>
    
</template>

<script>
export default{
    
Name: 'Productos',
    data(){
        return{
            fotos: [
                require ('../assets/Producto/o1.png'),
                require ('../assets/Producto/o1.png'),
                require ('../assets/Producto/o2.png'),
                require ('../assets/Producto/o3.png'),
                require ('../assets/Producto/o4.png') 
            ]
        }
    },
methods: {
    cambiofoto(id) {
        this.fotos[0] = this.fotos[id]
        }
    }
}
</script>


<style scoped>

/* General */

#Productos {
    border-radius: 25px;
    padding: 1rem;
    margin: 1rem;
    flex: 0 1 50%;
}

/* Imagen principal */

.principal {
    display: flex;
    justify-content: space-between;
    align-items: flex-start;
}

.principal img{
    height: 450px;
    align-items: center;
    padding-top: 1em;
}

/* Imagenes pequeñas */

.miniatura{
    border: 1px solid #cac8c8;
    width: 600px;
    margin-top: 2em;
    align-items: center;
    justify-content:center;
}

.miniatura img {
    width: 100px;
    padding: 1em;  
    margin-left: 1em;
    
}

</style>
