<template>
  <div>
    <Cabecera />
    <div class="barra">
      <MenuPrincipal class="menu" />
      <BarraBusqueda />
    </div>
    <div class="container">
      <CaminoMigas />
      <div class="dos-columnas">
        <ProductoImagen />
        <ProductoDatos />
      </div>
      <div class="descrip">
        <ProductoDescripcion />
      </div>
    </div>
    <Pie />
  </div>
</template>

<script>
import Cabecera from "./components/Cabecera.vue";
import MenuPrincipal from "./components/MenuPrincipal.vue";
import BarraBusqueda from "./components/BarraBusqueda.vue";
import CaminoMigas from "./components/CaminoMigas.vue";
import ProductoImagen from "./components/ProductoImagen.vue";
import ProductoDatos from "./components/ProductoDatos.vue";
import ProductoDescripcion from "./components/ProductoDescripcion.vue";
import Pie from "./components/Pie.vue";

export default {
  name: "App",
  components: {
    Cabecera,
    MenuPrincipal,
    BarraBusqueda,
    CaminoMigas,
    ProductoImagen,
    ProductoDatos,
    ProductoDescripcion,
    Pie,
  },
};
</script>

<style>
@import url("https://fonts.googleapis.com/css2?family=Roboto:wght@500&family=Titillium+Web:wght@300;400;700&display=swap");
/* Importo los iconos de material-design */
@import url("https://fonts.googleapis.com/css2?family=Material+Icons");

body {
  margin: 0px;
  padding: 0px;
  box-sizing: border-box;
}
.descrip {
  background: url("../public/nubes.jpg") #fff;
  z-index: 0;
  background-size: cover;
  background-repeat: no-repeat;
  background-position: center;
}

h1 {
  color: #bc1a42;
}
h2 {
  font-size: 1.7rem;
  color: #773149;
}
a,
a:hover,
a:visited {
  text-decoration: none;
  margin-left: 1rem;
  margin-right: 1rem;
  color: #bc1a42;
}
.barra {
  display: flex;
  background: #cacaca;
  justify-content: space-between;
  align-items: center;
  height: 4em;
}
.menu {
  flex-grow: 1;
}

#app {
  font-family: "Roboto", sans-serif;
}
.container {
  max-width: 1400px;
  margin: 0 auto;
}

.boton {
  background-color: #bc1a42;
  font-size: 1.2rem;
  font-weight: 700;
  color: white;
  padding: 0.7rem 1rem;
  cursor: pointer;
  border: none;
  border-radius: 1.3em;
}
.dos-columnas {
  display: flex;
  padding: 1rem;
  justify-content: center;
  flex-wrap: wrap;
}
</style>
