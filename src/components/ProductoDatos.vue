<template>
  <section id="producto-datos">
      <h1>Coche Tesla model Y</h1>
      <p>El Model Y es un coche de tamaño mediano completamente eléctrico con siete plazas, motor dual, tracción integral y una protección sin igual.</p>
      <p class="info">El precio mensual varía en función del número de años contratados (de 0 a 6 años). A partir de 6 años es constante.</p>
      <h2><span id="precio_r">625</span> <span class="uds">€/mes</span></h2>
      <div class="wrapper">
          <button class="btn" @click="cambiarContador('-1')" type="button" name="button">-</button>
          <input class="cantidad" type="text" name="name" :value="contador">
          <button class="btn" @click="cambiarContador('1')" type="button" name="button">+</button>
          <span> años de contrato renting</span>
      </div>
      <br>
      <button class="boton"><span class="material-icons">car_rental</span> Contratar</button>
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
            if (this.contador>0 && this.contador<8) {
              document.getElementById('precio_r').innerHTML= 625-(this.contador-1)*10;
            }
        }
    }


}
</script>

<style scoped>
#producto-datos {
  flex: 1 1 18rem;
}
h1 {
  font-size: 2.2rem;
}

.info {
  font-size: 0.9em;
  color: #bc1a42;
}

span.uds {
  font-size:1.3rem;
  font-weight: bold;
  color: #4d4d4d
}
.wrapper {
  height: 2rem;
  display: flex;
}

.wrapper span {
  margin-left: 0.5em;
}

.cantidad {
  border: none;
  text-align: center;
  width: 2rem;
  font-size: 1.2rem;
  background: none;
}
.btn {
  border: 2px solid #cacaca;
  width: 2rem;
  border-radius: 1.4em;
}
button:focus, input:focus {
  outline: 0;
}

</style>