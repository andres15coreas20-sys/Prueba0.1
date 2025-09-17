<template>
  <div class="contenedor">
    <h2>Comparación de Marcas de Laptops</h2>
    <table class="tabla">
      <thead>
        <tr>
          <th>Marca</th>
          <th>Rendimiento</th>
          <th>Precio Promedio</th>
          <th>Durabilidad</th>
        </tr>
      </thead>
      <tbody>
        <tr v-for="(marca, index) in marcas" :key="index">
          <td>{{ marca.nombre }}</td>
          <td>{{ marca.rendimiento }}</td>
          <td>{{ marca.precio }}</td>
          <td>{{ marca.durabilidad }}</td>
        </tr>
      </tbody>
    </table>
  </div>
</template>

<script setup>
const marcas = [
  { nombre: "Dell", rendimiento: "Alto", precio: "$1000", durabilidad: "Alta" },
  { nombre: "HP", rendimiento: "Medio", precio: "$850", durabilidad: "Media" },
  { nombre: "Lenovo", rendimiento: "Alto", precio: "$950", durabilidad: "Alta" },
  { nombre: "Acer", rendimiento: "Medio", precio: "$700", durabilidad: "Media" },
]
</script>

<style scoped>
.tabla {
  border-collapse: collapse;
  width: 100%;
}
.tabla th, .tabla td {
  border: 1px solid #ccc;
  padding: 8px;
  text-align: center;
}
</style>
