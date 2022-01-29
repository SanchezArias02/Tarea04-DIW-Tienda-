<template>
    <section id="barra-menu">
        <div class="super-top"><li><span>ENVIOS</span> totalmente gratis a partir de 29€</li></div>
        <div class="top">
            <ul>
                <li><a href="#">Servicios</a></li>
                <li><a href="#">Marcas</a></li>
                <li><a href="#">Tiendas</a></li>
                <li><a href="#">Trabaja con nosotros</a></li>
                <li><a href="#">Preguntas frecuentes</a></li>
            </ul>
            <div id="mid">
                <div class="busqueda">
                    <span class="icono"><a href="#"><img class="fav" src="../assets/Iconos-img/busqueda.png" alt="Lupa" copyright="cc-by Icono lupa"/></a></span>
                    <input type="search" id ="buscar" placeholder="¿Qué deseas buscar?"/>
                </div>
            </div>
            <div class="grow"></div>
            <div class="expan">
                <nav>
                    <ul>
                        <li>
                            <div class="iconos-flx">
                                <img src="../assets/Iconos-img/caja.png" alt="Pedidos" copyright="cc-by Icono pedidos" height="22"/>
                                <div class="iconos">Gestionar<br> pedidos</div>
                            </div>
                        </li>
                        <li>
                            <div class="iconos-flx">
                                <img src="../assets/Iconos-img/persona.png" alt="Inicio sesion" copyright="cc-by Inicio sesion" height="22"/>
                                <div class="iconos">Registrarse<br> o loguearse</div>
                            </div>
                        </li>   
                        <li>
                            <div class="iconos-flx">
                                <img src="../assets/Iconos-img/Cesta.png" alt="Carrito compra" copyright="cc-by Carrito compras" height="22"/>
                                <div class="iconos">Carrito de<br> compras</div>
                            </div>
                        </li>    
                    </ul>
                </nav>
            </div>
        </div>
        <div class="bottom">
            <div class="left">
                <img src="../assets/Logotipos/Inse-Tech.png" alt="Empresa Inse-Tech" copyright="c Andrés Sánchez Arias" height="90px" width="300px"/>
                <header>
                    <!-- ≡  Categorias productos -->
                        <nav class="navegacion">
                            <ul class="menu">
                               <li><a href="#">Ofertas</a></li>
                               <li><a href="#">Ordenadores</a>
                                    <ul class="submenu">
                                        <li><a href="#">Portátiles</a></li>
                                        <li><a href="#">Sobremesa</a></li>
                                        <li><a href="#">SuperOrdenadores</a></li>
                                        <li><a href="#">Servidores</a></li>
                                    </ul>
                                </li>
                               <li><a href="#">Televisión</a>
                                    <ul class="submenu">
                                        <li><a href="#">22"</a></li>
                                        <li><a href="#">32"</a></li>
                                        <li><a href="#">40" o 43"</a></li>
                                        <li><a href="#">50"</a></li>
                                        <li><a href="#">63" a más</a></li>
                                    </ul>
                               </li>
                               <li><a href="#">Audio</a></li>
                               <li><a href="#">Telefonía</a></li>
                               <li><a href="#">Electrodomésticos</a></li>
                            </ul>
                        </nav>
                </header>
            </div>
        
            <div class="grow"></div>
            <div class="right">
                    ¿Necesitas ayuda? <div class="chatea"> <img src="../assets/Iconos-img/tlf.png" alt="Teléfono" copyright="cc-by Icono telefono"/>Chatea con nosotros</div>
               
            </div>
        </div>
    </section>

</template>

<script>

</script>

<style scoped>

    @import url('https://fonts.googleapis.com/css2?family=Mukta:wght@400;500&display=swap');
    
/* Envios gratis */

    .super-top{ background:rgb(207, 216, 200); padding: 0.5em;   }
    
    .super-top li {
        list-style: none; 
        color:white; 
        text-align: center;
        font-size: 16px;
        font-weight: bold; 
        
    } 

    .super-top li span{
        letter-spacing: 1pt;
        font-size: 18px;
    }
    
/* Menú superior */

    section#barra-menu{
        background:#f8f9f9;
        font-family: 'Mukta', sans-serif;
    }

    .top{
        display:flex;
    }

    .top ul{
        list-style: none;
        display:flex;

    }

    .top ul li{
        display:block;
        margin: 0 0.5em 0 0.5em;
    }

    .top ul li a{
        text-decoration: none;
        color: #63717f;
        text-decoration: none;
        position: relative;
        
    }

    .top ul li a::before{ 
        content: '';
        position: absolute;
        bottom: 0;
        left: 0;
        width: 100%;
        height: 1.5px;
        background: linear-gradient(to right, #8c6363, #c1b6cf, #e9d2e9);
        z-index: 1;
        transform: scaleX(0);
        transform-origin: center;
        transition: transform 0.5s ease-in-out;
    }

    .top ul li a:hover::before{
        transform: scaleX(1);
    }

    .grow{
        flex-grow: 1;
    }

/* Menu de navegacion principal */
    .navegacion{
        width: 750px;
        margin: 20px auto;
        margin-left: 2em;
        background:rgb(58, 57, 57);
        border-radius: 10px;
    }

    .navegacion ul{
        list-style: none;
    }

    .menu > li{
         /* position: relative; */
         display: inline-block;
    }

    .menu > li > a{
        display: block;
        padding: 15px 20px;
        color:#ffffff;
        text-decoration: none;
        justify-content: space-around;
        
    }

    .menu li a:hover{
        color:rgb(220, 213, 221);
        transition: all .3s;
    }

/* Menu principal > submenus */

    .submenu{
        position: absolute;
        background-color:#333333;
        visibility: hidden;
        opacity: 0;
        transition: all 0.4s;
        
    }

    .submenu li a{
        display:block;
        padding: 15px;
        color: #ffffff;
        text-decoration: none;   
    }

    .menu li:hover .submenu{
       visibility:visible;
       opacity:1;
        
    }

/*Iconos pedidos */

    .iconos-flx{ 
        display:flex;
        align-items:center;
    }

    .iconos-flx:hover{
        background-color:white;
        transition: all 0.5s;
        padding: 0.1em;
        border-radius: 10px;
    }

    .iconos{
        line-height:8pt;
        font-size: 12px;
        margin: 0 1.5em 0 1.2em;
        position: relative;
        padding:0.5em;
        justify-content:center;
    }

     .iconos-flx div::after{
        content: "|";
        font-size: 24px;
        color: rgb(116, 116, 116);
        margin: 0 0 0 0.5em;
    }



/*Seccion inferior */

.bottom{
    display:flex;
    align-items:center;
}

.left{
    display:flex;
    align-items:center;
}

.left img{
    border-radius:10px;
    margin: 0 0 0 1em;
}


/* Barra busqueda */

.mid input{
    height:40px;
    width:500px;
    border-radius: 5px;
    outline: none;
    border: 1px solid white;
}

.mid button{
    height:40px;
    width:60px;
    margin: 0 0 0 0.5em;
    border-radius: 5px;
    outline: none;
    background:rgb(231, 230, 230);
    color:rgb(71, 66, 66);
    font-weight: bold;
}

 #mid .busqueda{
        width: 300px;
        vertical-align: middle;
        white-space: nowrap;
        position: relative;
        margin: 0.6em 0 0 0;
    }

    .busqueda input#buscar{
        width: 450px;
        height: 50px;
        background: rgb(243, 243, 243);
        border: none;
        font-size: 15px;
        float: left;
        color: #33393f;
        padding-left: 45px;
        border-radius: 5px;
        margin: 0 0 0 1em;
    }

     .busqueda .fav{
        position: absolute;
        top: 60%;
        margin-left: 30px;
        margin-top: 17px;
        z-index: 1;
        width: 05%;
    }

    .busqueda .icono{
        position: absolute;
        top: 60%;
      
        color: #4f5b66;
        width: 100%;
    }

/* Chatea con nosotros */

.right {
   margin: 0 3em 0 0;
   align-items: center;
}

.right .chatea{
    display: inline-block;
    background-color:rgb(233, 178, 201);
    color:rgb(255, 255, 255);
    padding: 0.5em;
    border-radius: 20px;
    border: 3px solid rgb(255, 197, 224);
    margin: 0 0 0 0.5em;
}

.right .chatea img{
    align-items: center;
    width:20px;
    vertical-align: middle;
    margin: 0 0.5em 0 0;

}


</style>
