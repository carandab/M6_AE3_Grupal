# Ejercicio Grupal: App de Recetas con Django

---

## 🎯 **Objetivo**

Construir en equipo un sitio web dinámico de recetas utilizando **Django**. Cada integrante será responsable de una parte del proyecto, aplicando los conceptos de **MVC/MTV**, navegación, contenido estático y dinámico, y diseño responsivo con **Bootstrap**.

---

## 🌐 **Contexto del Proyecto**

La **App de Recetas** es un sitio web donde los usuarios pueden ver y explorar diversas recetas de cocina. El proyecto debe incluir:
- Página de inicio con lista de recetas
- Página individual para cada receta con detalles
- Página de contacto
- Diseño visualmente atractivo y completamente funcional usando Bootstrap

---

## 📋 **Requisitos del Proyecto**

### 1. **Estructura del Proyecto**
- **Navbar:** Barra de navegación para acceder a "Inicio", "Recetas" y "Contacto".
- **Jumbotron:** En la página de inicio, resalta el propósito del sitio.
- **Footer:** Pie de página con información adicional y derechos de autor.

### 2. **Páginas Estáticas y Dinámicas**
- **Inicio:** Mensaje de bienvenida y lista de las últimas recetas (nombre y breve descripción).
- **Recetas:** Página individual para cada receta (nombre, ingredientes, instrucciones, imagen). Información dinámica desde la base de datos.
- **Contacto:** Formulario para que los usuarios envíen un mensaje.

### 3. **Navegación y Responsividad**
- Todas las páginas deben estar conectadas mediante la barra de navegación.
- El sitio debe ser **responsivo** (adaptable a móviles y escritorio).

### 4. **Contenido Estático**
- **Imágenes:** Cada receta debe tener una imagen estática almacenada en la carpeta de archivos estáticos de Django.
- **CSS personalizado:** Además de Bootstrap, puedes crear un archivo CSS propio para personalizar el sitio.

### 5. **Modelos y Vistas**
- Crea un modelo `Receta` con los siguientes campos:
  - `nombre` (CharField)
  - `ingredientes` (TextField)
  - `instrucciones` (TextField)
  - `imagen` (ImageField)
- Utiliza **vistas genéricas** para mostrar las recetas.
- La página de inicio debe mostrar una lista de recetas. Al hacer clic en una receta, redirige al usuario a la página de detalles.

### 6. **Plantillas (Templates)**
- Utiliza **herencia de templates** para evitar repetición de código.
  - El navbar y el footer deben estar en un template base.
  - Las demás páginas deben extender este template base.
- En la página de Recetas, usa un ciclo `for` para mostrar todas las recetas.
- En la página de Detalles de Receta, utiliza condiciones `if/else` para mostrar la receta solo si existe.

### 7. **Redirección y Manejo de Errores**
- Si una receta no existe, redirige al usuario a una **página de error personalizada**.
- Si el usuario intenta acceder a la página de contacto sin completar el formulario, muestra un **mensaje de advertencia**.

### 8. **Enlaces de URL y Redirección**
- Utiliza **etiquetas URL** en los templates para URLs dinámicas.
- Al enviar el formulario de contacto, redirige al usuario a una **página de confirmación**.

---

## 📦 **Entrega**
- Entregar un archivo **zip** con los archivos del proyecto o un **repositorio en Github**.
- **Duración:** 1 jornada de clases.
- **Ejecución:** Grupal.