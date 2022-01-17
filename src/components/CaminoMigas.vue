<template>
  <section id="camino-migas">
      <a href="#"><span class="material-icons">home</span> INICIO </a>
      <a href="#">ELECTRICOS</a> 
      <a class="actual" href="#">TESLA</a> 


  </section>
</template>

<script>
export default {

}
</script>

<style scoped>

#camino-migas {
display: flex;
border-radius: 10px;
margin: auto;
height: 1em;
z-index: 1;
justify-content: start;
margin-left: 1em;
}

.actual {
  text-decoration-line: underline;
  text-decoration-color: #cacaca;
  color: #bc1a42;
}

a {
height: 100%;
background-color: white;
color: #cacaca;
font-family: Arial, Helvetica, sans-serif;
border-radius: 7px;
letter-spacing: 1px;
transition: all 0.3s ease;
text-transform: uppercase;
position: relative;
display: inline-flex;
justify-content: center;
align-items: center;
font-size: 0.7em;
transform: skew(-21deg);
box-shadow: 0 2px 5px rgba(0,0,0,0.26);
margin: 5px;
padding: 0.7em;
cursor: pointer;
}

a:hover {
background: #bc1a42;
color: #FFF;
}
</style>