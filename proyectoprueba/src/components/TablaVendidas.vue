<template>
  <div class="contenedor">
    <h2>Laptops Vendidas</h2>
    <table class="tabla">
      <thead>
        <tr>
          <th>ID Venta</th>
          <th>Marca</th>
          <th>Modelo</th>
          <th>Precio (USD)</th>
          <th>Fecha</th>
        </tr>
      </thead>
      <tbody>
        <tr v-for="(venta, index) in ventas" :key="index">
          <td>{{ venta.id }}</td>
          <td>{{ venta.marca }}</td>
          <td>{{ venta.modelo }}</td>
          <td>{{ venta.precio }}</td>
          <td>{{ venta.fecha }}</td>
        </tr>
      </tbody>
    </table>
  </div>
</template>

<script setup>
const ventas = [
  { id: 1, marca: "Dell", modelo: "XPS 13", precio: 1200, fecha: "2025-09-01" },
  { id: 2, marca: "HP", modelo: "Pavilion 15", precio: 800, fecha: "2025-09-05" },
  { id: 3, marca: "Lenovo", modelo: "ThinkPad X1", precio: 1400, fecha: "2025-09-10" },
  { id: 4, marca: "Acer", modelo: "Aspire 5", precio: 650, fecha: "2025-09-12" },
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
