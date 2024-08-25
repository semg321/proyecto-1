<script lang="ts" setup>

import { devices } from '~/server/api/devices.json'

</script>

<template>
  <div>
    <h1>Dispositivos</h1>
    <div class="grid">
      <Card v-for="device in devices" :key="device.id" :="device"/>
    </div>
  </div>
</template>

<style scoped>
.grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(18rem, 1fr));
  gap: 2rem;
}
</style>
