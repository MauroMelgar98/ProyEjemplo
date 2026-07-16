<script setup>
import { ref } from 'vue'

const nombre = ref('')
const telefono = ref('')

const clientes = ref([])

function guardarCliente() {

    clientes.value.push({
        nombre: nombre.value,
        telefono: telefono.value
    })

    nombre.value = ''
    telefono.value = ''
}
</script>

<template>

<h2>Registro de Clientes</h2>

<input
    v-model="nombre"
    placeholder="Nombre">

<input
    v-model="telefono"
    placeholder="Teléfono">

<button @click="guardarCliente">
    Guardar
</button>

<hr>

<ul>

<li
v-for="cliente in clientes">

{{ cliente.nombre }}
-
{{ cliente.telefono }}

</li>

</ul>

</template>