<script setup>
import EncabezadoApp from './components/EncabezadoApp.vue';
import FormularioClientes from './components/FormularioClientes.vue';

</script>
<!-- import EncabezadoApp from '.components/EncabezadoApp.vue' -->

<template>
  <EncabezadoApp
    titulo="Gestion de Emprendimientos"
    subtitulo="Proyecto de Programacion Web II"
  />

<main>
  <h1> Modulos prinpipales </h1>
  <p> Clientes, productos,ventas e inventario </p>
</main>
</template>

<style scoped>
main {
max-width: 900px;
margin: 40px auto;
font-family: Arial, sans-serif;
}
h1 {
  margin-bottom: 8px;
}
</style>
