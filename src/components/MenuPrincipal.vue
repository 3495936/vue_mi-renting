<template>
<section id="menu-principal">
    <div class="container">
    <nav>
            <a href="#">INICIO</a>
            <a href="#">TURISMOS</a>
            <a href="#">SUV</a>
            <a href="#">COMPACTOS</a>
            <a href="#">ELECTRICOS</a>
    </nav>
    <div class=registrados>
        <a class="registro" href="#"><span class="material-icons">face</span><br> REGISTRO</a>
        <a class="login" href="#"><span class="material-icons">login</span><br> LOG-IN</a>
    </div>
</div>
</section>

  
</template>

<script>
export default {

}
</script>

<style scoped>
#menu-principal {    
    display: flex;
    z-index:999;
    justify-content: space-around;
    min-width: 737px;
}
.container {
    display: flex;
    justify-content: space-around;
}
nav {
    display:flex;
    list-style: none;
    padding: 0.3rem;
    text-align: center;
    align-items: center;
}
.registrados {
    color: #bc1a42;
    display: flex;
    flex-flow: row nowrap;
    justify-content: end;
    align-items: center;
    text-align: center;
    padding: 0.3rem;
    min-width: 190px;
    margin-left: 1.5em;
}
nav a, .registrados a {    
    text-decoration: none;
    font-weight: 700;
    color:white;
}
.registrados a {
    color:#bc1a42;
}
nav a:hover,.active, .registrados a:hover {
    text-decoration: none;
    font-weight: 700;
    padding-top: 0.5rem;
}




</style>