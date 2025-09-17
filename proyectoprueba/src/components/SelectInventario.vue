<template>
  <div class="contenedor">
    <h2>Inventario de Marcas</h2>
    <select v-model="marcaSeleccionada">
      <option disabled value="">Seleccione una marca</option>
      <option v-for="(marca, index) in inventario" :key="index" :value="marca">
        {{ marca }}
      </option>
    </select>

    <p v-if="marcaSeleccionada">Marca seleccionada: <b>{{ marcaSeleccionada }}</b></p>
  </div>
</template>

<script setup>
import { ref } from "vue"

const inventario = ["Dell", "HP", "Lenovo", "Acer", "Asus"]
const marcaSeleccionada = ref("")
</script>

<style scoped>
select {
  padding: 6px;
  margin-top: 10px;
}
</style>
