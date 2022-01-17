<template>
  <section id="barra-busqueda">
      <form @submit.prevent="handleEnviar">
          <input type="text" placeholder="Buscar coche ...">
          <button class="boton"><span class="material-icons">search</span></button>
      </form>
  </section>
</template>

<script>
export default {
    name: 'BarraBusqueda',
    methods: {
        handleSutmit() {
            console.log("Busqueda enviada")
        }
    }
}
</script>

<style scoped>
form {
    display: flex;
    justify-content: center;
    align-items: center;
}
input{
    margin: 0.5rem;
    padding: 0.7rem 1rem;
    border-style: solid;
    border: 2px solid #bc1a42;
    color: #181818;
    outline: none;
    line-height: 1.4rem;
    border-radius: 25px;
    font-size: 1.2rem;
    flex: 0 1 160px;
    min-width: 160px;
}


</style>