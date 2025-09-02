<template>
    <h1 class="text-center my-4">Lista de Usuarios</h1>
  <table class="table table-striped table-hover align-middle text-center">
    <thead class="table-light">
      <tr>
        <th>#</th>
        <th>Nombre</th>
        <th>Apellido</th>
        <th>Fecha de nacimiento</th>
        <th>Edad</th>
      </tr>
    </thead>

    <tbody>
      <tr v-for="(u, idx) in usuarios" :key="u.id">
        <td>{{ idx + 1 }}</td>
        <td>{{ u.nombre }}</td>
        <td>{{ u.apellido }}</td>
        <td>{{ formatFecha(u.fechaNac) }}</td>
        <td>{{ u.edad }}</td>
      </tr>
    </tbody>
  </table>
</template>

<script setup>
import { reactive } from 'vue'

// Estado reactivo: ref() hace que Vue escuche cambios
const usuarios = reactive([
  { id: 1, nombre: 'Nelson', apellido: 'Valenzuela', fechaNac: '1993-05-12', edad: 32 },
  { id: 2, nombre: 'Ana',    apellido: 'Gómez',      fechaNac: '1989-11-02', edad: 35 },
  { id: 3, nombre: 'Luis',   apellido: 'Pérez',      fechaNac: '2001-03-25', edad: 24 },
])

// Funciones normales: se pueden usar directo en el template
function formatFecha(iso) {
  const d = new Date(iso + 'T00:00:00')
  return new Intl.DateTimeFormat('es-CL', { dateStyle: 'long' }).format(d)
}
</script>