<template>
  <section id="producto-imagen">
      <div class="img-big">
          <figure>
          <img class="img-ppal" v-bind:src="fotos[0]" alt="Coche Turismo Tesla model Y" copyright="cc Pixabay License">
          <figcaption><a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Licencia Creative Commons" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a> <br />
          <a href="https://pixabay.com/es/images/search/tesla/">Pixabay License</a>
            </figcaption>
            </figure>
      </div>
        <div class="img-mini">
          <a @click="cambiarFoto(1)"><img  v-bind:src="fotos[1]" alt="Coche Turismo Tesla model Y"></a>
          <a @click="cambiarFoto(2)"><img  v-bind:src="fotos[2]" alt="Coche Turismo Tesla model Y"></a>
          <a @click="cambiarFoto(3)"><img  v-bind:src="fotos[3]" alt="Coche Turismo Tesla model Y"></a>
          <a @click="cambiarFoto(4)"><img  v-bind:src="fotos[4]" alt="Coche Turismo Tesla model Y"></a>
        </div>
      </section>    
</template>

<script>
export default {
  Name: "ProductoImagen",
  data() {
    return {
      fotos: [
        require("../assets/tesla1.jpg"),
        require("../assets/tesla1.jpg"),
        require("../assets/tesla2.jpg"),
        require("../assets/tesla3.jpg"),
        require("../assets/tesla4.jpg"),
      ],
    };
  },
  methods: {
    cambiarFoto(id) {
      this.fotos[0] = this.fotos[id];
    },
  },
};
</script>

<style scoped>
figcaption {
    align-self: center;
    text-align: center;
    background-color: #d8d8d878;
    font-size: 0.8em;
    padding-top: 0.5em;
}
.img-ppal{
    width: 700px;
}

#producto-imagen {
  border-radius: 25px;
  padding: 1rem;
  margin: 0;
  flex: 0 1 50%;
}
.img-mini {
  display: flex;
  justify-content: space-around;
  align-items: flex-start;
}
.img-mini img {
  width: 100px;
  border: 2px solid #d8d8d8;
  border-radius: 10px;
}

</style>