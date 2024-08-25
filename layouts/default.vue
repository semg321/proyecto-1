<template>
  <div class="d-flex">
    <Sidebar />
    <div class="content-wrapper flex-grow-1">
      <HeaderBar />
      <main class="pt-5"> <!-- Ajuste para el espacio bajo el HeaderBar -->
        <slot></slot>
      </main>
    </div>
  </div>
</template>

<script setup>
import Sidebar from '~/components/Sidebar.vue';
import HeaderBar from '~/components/HeaderBar.vue';
</script>

<style scoped>
.content-wrapper {
  margin-left: 250px; /* Ancho del Sidebar para que el contenido no se solape */
  padding: 15px; /* Agrega espacio alrededor del contenido */
}
</style>
