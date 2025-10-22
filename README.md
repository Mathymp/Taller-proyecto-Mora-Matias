# LOTIFY - Taller de Proyecto de Especialidad

**Autor:** Matias Mora Duran
**Asignatura:** Taller de Proyecto de la Especialidad
**Carrera:** Técnico en Programación y Análisis de Sistemas
**Docente:** Víctor M. Valderrama M.
**Semestre:** 2025-2

---

## 1. Descripción del Problema y Solución

### Problema 

Las pequeñas y medianas empresas (PYMEs) del sector inmobiliario y agrícola carecen de una herramienta accesible y autogestionable para crear recorridos virtuales 360° de sus loteos y parcelas. Actualmente, dependen de servicios externos costosos, lentos y rígidos. Si la empresa necesita actualizar un precio o marcar un lote como "Vendido", debe volver a contratar al proveedor, generando retrasos y costos adicionales.

### Solución Propuesta 

**LOTIFY** es una plataforma web (SaaS) que entrega el control total al cliente. Permite a usuarios no técnicos subir sus propias imágenes 360°, y (esta es la innovación) **dibujar polígonos vectoriales** directamente sobre la esfera 3D para demarcar lotes.

Además, permite importar archivos KMZ, añadir etiquetas interactivas (precio, metraje, estado) y gestionar esta información desde un panel de "edición rápida". La plataforma genera un Iframe para que la empresa pueda incrustar este visor dinámico en su propio sitio web, transformando un tour estático en una herramienta de gestión de inventario visual y en tiempo real.

## 2. Tecnologías Utilizadas 

* **Frontend:** HTML5, CSS3 (Bootstrap 5), JavaScript (Vanilla)
* **Librería 360 (Core):** Photo Sphere Viewer.js (basada en Three.js)
* **Backend:** Node.js, Express.js
* **Base de Datos:** **MySQL 8.0** (Diseño relacional normalizado)
* **Autenticación:** JSON Web Tokens (JWT)

## 3. Instrucciones Básicas de Uso 

Este sistema está diseñado para ser autogestionado por la empresa cliente (ej. una inmobiliaria). El flujo de uso principal es:

1.  **Registro/Login:** La empresa se registra en la plataforma LOTIFY.
2.  **Crear Proyecto:** Desde su panel de administración, crea un nuevo proyecto (ej. "Loteo Los Álamos").
3.  **Subir Imagen:** Carga la imagen 360° (tomada con dron o cámara 360) para ese proyecto.
4.  **Editar:** Accede al "Editor 360" donde puede:
    * Dibujar los polígonos de los lotes sobre la imagen.
    * Opcionalmente, importar un archivo KMZ para superponer los lotes.
    * Añadir hotspots de información (contacto, precios, etc.).
5.  **Gestionar Datos:** En el panel "Edición Rápida", asigna precios, metraje y estado ('Disponible', 'Vendido') a cada lote dibujado.
6.  **Publicar:** El sistema genera un enlace público y un código `<iframe>`.
7.  **Incrustar:** El cliente copia el `<iframe>` y lo pega en su propio sitio web para que los visitantes lo vean.

## 4. Documentación y Licencia 

* **Informe Avance 1:**
    * `[Ver Informe PDF en /documentos/]`
* **Diagrama de Procesos (DFD):**
    * `[Ver Diagrama en /diagramas/]`
* **Licencia:**
    * Este proyecto académico se distribuye bajo la **Licencia MIT**. Ver el archivo `LICENSE` en la raíz del repositorio para más detalles.
