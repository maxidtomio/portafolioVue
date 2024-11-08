<script setup>
import NavBar from './components/NavBar.vue';
import ComponenteProyectos from './components/ComponenteProyectos.vue';
import ComponenteEducacion from './components/ComponenteEducacion.vue';
import ComponenteContacto from './components/ComponenteContacto.vue';
import ComponenteAbout from './components/ComponenteAbout.vue';
</script>

<template>
 <header>
    <NavBar />
  </header>
  <main>
    <section id="about">
      <h2>Sobre mi</h2>
      <ComponenteAbout />
    </section>
    <section id="educacion">
      <h2>Educación</h2>
      <ComponenteEducacion />
    </section>
     <section id="proyectos">
      <h2>Proyectos</h2>
      <ComponenteProyectos />
    </section>
    <section id="contacto">
      <h2>Contacto</h2>
      <ComponenteContacto />
    </section>
  </main>

  <footer>
    <a href="#top">
      <button class="botonInicio">Inicio</button>
    </a>
    <p>© Maximiliano Tomio - Portafolio Web - UTN FRSR 2024</p>
  </footer>
</template>

<style scoped>

</style>
