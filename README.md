# Proyecto VueJS -- M6AE1 ABP1

Este proyecto corresponde a la actividad **"Introducción al Framework
VueJS"** del módulo 6.\
Su objetivo es construir una aplicación simple utilizando Vue 3 y
Bootstrap para mostrar una tabla de usuarios, comprendiendo los
fundamentos del framework orientado a componentes.

## 🎯 Aprendizaje Esperado

> Describir los aspectos fundamentales de un framework orientado a
> componentes para el desarrollo de una aplicación Front-End.

## 📋 Requerimientos de la Actividad

-   Mostrar en pantalla una tabla de usuarios con los siguientes datos:
    -   Nombre\
    -   Apellido\
    -   Fecha de Nacimiento\
    -   Edad\
-   Los datos deben estar almacenados en la `data` (estado reactivo) del
    componente de VueJS y renderizados directamente en la tabla.\
-   Se recomienda el uso de **arreglos y objetos** para simplificar el
    código.\
-   La tabla debe usar **Bootstrap** para darle estilo.

## 🛠️ Tecnologías utilizadas

-   [Vue 3](https://vuejs.org/) (Composition API con `<script setup>`).\
-   [Bootstrap 5](https://getbootstrap.com/) para los estilos de la
    tabla.

## 🚀 Instalación y ejecución del proyecto

1.  Clona el repositorio o descarga el .zip.\

2.  Instala las dependencias:

    ``` bash
    npm install
    ```

3.  Inicia el servidor de desarrollo:

    ``` bash
    npm run dev
    ```

4.  Abre la URL que te indique Vite (por lo general
    `http://localhost:5173/`).

## 📂 Estructura del proyecto

   .
    ├── src/
    │   ├── components/
    │   │   └── UsersTable.vue
    │   ├── App.vue
    │   └── main.js
    ├── .gitignore
    ├── index.html
    ├── package.json
    ├── package-lock.json
    ├── README.md
    ├── vite.config.js
    └── jsconfig.json

-   **App.vue**: componente principal que carga la vista general.\
-   **UsersTable.vue**: componente que contiene la tabla y la data
    reactiva de usuarios.

## ✨ Resultado esperado

Al ejecutar la aplicación se debe mostrar una tabla con tres usuarios
ficticios, mostrando sus nombres, apellidos, fechas de nacimiento y
edades.\
La tabla incluye estilos de Bootstrap (`table`, `table-striped`,
`table-hover`, etc.).

## 📦 Entregable

De acuerdo a la consigna, se debe entregar la carpeta del proyecto
comprimida en formato `.zip`.

------------------------------------------------------------------------

📚 *Actividad realizada como parte del programa de Talento Digital --
Módulo 6.*