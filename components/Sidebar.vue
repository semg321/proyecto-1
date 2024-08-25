<template>
  <nav class="navbar bg-dark text-white d-flex flex-column position-fixed" style="height: 100vh; width: 250px;">
    <h1 class="text-white m-0">NGIOT</h1>
    <ul class="navbar-nav d-flex flex-column flex-grow-1 justify-content-start gap-3 w-100">
      <li class="nav-item">
        <NuxtLink class="btn btn-outline-light d-flex align-items-center text-start" to="/" active-class="active">
          <Icon name="lucide:house" size="24px" class="me-2" />
          Inicio
        </NuxtLink>
      </li>
      <li class="nav-item">
        <NuxtLink class="btn btn-outline-light d-flex align-items-center text-start" to="/devices" active-class="active">
          <Icon name="bx:devices" size="24px" class="me-2" />
          Dispositivos
        </NuxtLink>
      </li>
      <li class="nav-item">
        <NuxtLink class="btn btn-outline-light d-flex align-items-center text-start" to="/monitoring" active-class="active">
          <Icon name="ic:outline-monitor-heart" size="24px" class="me-2" />
          Monitoreo
        </NuxtLink>
      </li>
      <li class="nav-item">
        <NuxtLink class="btn btn-outline-light d-flex align-items-center text-start" to="/contact" active-class="active">
          <Icon name="teenyicons:contact-outline" size="24px" class="me-2" />
          Contacto
        </NuxtLink>
      </li>
    </ul>
  </nav>
</template>

<style scoped>
/* Estilos del Sidebar */
h1 {
  font-size: 2rem;
  padding: 40px;
}

.navbar-nav {
  gap: 1rem;
}

.nav-item {
  margin: 0;
  padding: 0 20px;
}

.btn-outline-light {
  border: none;
  color: white;
  padding: 10px;
}

.btn-outline-light:hover {
  background-color: white;
  color: black;
}

.me-2 {
  margin-right: 0.5rem;
}

.active {
  color: black;
}

.active:hover {
  background-color: #212529;
  color: white;
}
</style>
