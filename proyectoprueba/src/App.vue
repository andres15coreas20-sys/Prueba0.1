<template>
  <div>
  <TablaComparacion/>
  <SelectInventario/>
  <TablaVendidas/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import SelectInventario from './components/SelectInventario.vue';
import TablaComparacion from './components/TablaComparacion.vue';
import TablaVendidas from './components/TablaVendidas.vue';

export default {
  name: 'App',
  components: {
    HelloWorld
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
