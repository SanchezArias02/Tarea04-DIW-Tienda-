<template>
  <div class="contenedor">
    <MenuPrincipal/>
    <Breadcrumbs/>
      <div class="ProductoPago">
        <Productos/>
        <ZonaPago/>
      </div>
    <ProductoDescripcion/>
    <Pie/>
  </div>
</template>

<script>
import Breadcrumbs from './components/Breadcrumb.vue'
import Productos from './components/Productos.vue'
import ZonaPago from './components/ZonaPago.vue'
import ProductoDescripcion from './components/ProductoDescripcion.vue'
import Pie from './components/Pie.vue'
import MenuPrincipal from './components/MenuPrincipal.vue'

export default {
  name: 'App',
  components: { 
    MenuPrincipal,
    Breadcrumbs,
    Productos,
    ZonaPago,
    ProductoDescripcion,
    Pie,
   
  }
}
</script>

<style>
@import './assets/CSS/styles.css';
</style>
