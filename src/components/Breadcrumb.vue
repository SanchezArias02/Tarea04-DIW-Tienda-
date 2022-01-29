<template>
    <section id="navegacion">
        <div class="migaspan">
            <li class="listar-migas">
                <a href="#"> Inicio </a> 
            </li>    
            <li class="listar-migas">
                <a href="#">Informática</a> 
            </li>
            <li class="listar-migas">
                <a href="#">Ordenadores</a> 
            </li>
            <li class="listar-migas"> 
                <a class="enlace--activo" href="#"><strong>Portátiles</strong></a>
            </li>
        </div>
    </section>
</template>

<script>

export default{

}

</script>

<style scoped>

section#navegacion .migaspan{
    display:flex;
    padding: 10px;
    align-items:center; 
    font-size: 15px;  
}

section#navegacion .listar-migas{
    display:inline-block;
    font-family: "Montserrat", sans-serif;
}

.listar-migas:not(:last-of-type)::after{
    content: "/";
    margin: 0 5px;
    color: rgb(80, 79, 79);
}


.listar-migas a{
    text-decoration: none;
    position: relative;
    color: rgb(59, 59, 59);
    padding: 5px;
}

.listar-migas a::before{
    content: '';
    position: absolute;
    bottom: 0;
    left: 0;
    width: 100%;
    height: 2px;
    background: linear-gradient(to right, #494e50, #505d5e, #678585);
    z-index: 1;
    transform: scaleX(0);
    transform-origin: left;
    transition: transform 0.5s ease-in-out;
}

.listar-migas a:hover::before{
    transform: scaleX(1);
}

</style>
