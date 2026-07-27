# Guía rápida — Publicar la web de la Escuela de Invierno en GitHub

Esta web es un solo archivo (`index.html`). Cuando la publiques en GitHub Pages,
lista **automáticamente** los archivos que subas a las carpetas de cada curso.
No necesitas editar código: subes un archivo → aparece para descargar.

Tiempo estimado: ~5 minutos.

---

## Paso 1 — Crear el repositorio

1. Entra a <https://github.com> con tu cuenta.
2. Arriba a la derecha, haz clic en **+** → **New repository**.
3. En **Repository name** escribe, por ejemplo: `escuela-invierno-ipe`
4. Déjalo en **Public** (necesario para que GitHub Pages sea gratis y accesible).
5. **No** marques "Add a README" (ya lo traemos incluido).
6. Clic en **Create repository**.

---

## Paso 2 — Subir los archivos del sitio

En la página del repositorio recién creado:

1. Haz clic en **uploading an existing file** (enlace en el centro), o en
   **Add file → Upload files**.
2. Arrastra **todo el contenido** de la carpeta `escuela-invierno-ipe` que te
   entregué (el archivo `index.html`, `README.md`, y la carpeta `material/`
   completa con sus subcarpetas).
   - Si arrastras la carpeta completa, GitHub conserva la estructura.
3. Abajo, clic en **Commit changes**.

> La carpeta `material/` trae dos subcarpetas vacías (`microeconometria` y
> `macroeconometria`) con un archivo técnico `.gitkeep`. Ese archivo solo sirve
> para que GitHub conserve la carpeta vacía; puedes ignorarlo.

---

## Paso 3 — Activar GitHub Pages

1. En el repositorio, ve a **Settings** (arriba a la derecha).
2. En el menú lateral izquierdo, clic en **Pages**.
3. En **Source**, elige **Deploy from a branch**.
4. En **Branch**, selecciona **main** y carpeta **/ (root)**. Clic en **Save**.
5. Espera 1–2 minutos. Recarga la página de **Pages**: arriba aparecerá la
   dirección pública, algo como:

   ```
   https://TU-USUARIO.github.io/escuela-invierno-ipe/
   ```

Esa es la dirección que compartes con los estudiantes. ✅

---

## Paso 4 — Subir material de cada curso (lo harás cada vez que tengas algo nuevo)

1. En el repositorio, entra a la carpeta `material` → luego al curso, por
   ejemplo `microeconometria`.
2. Clic en **Add file → Upload files**.
3. Arrastra los archivos (PDF, slides, datos, código R/Stata, lo que sea).
4. Clic en **Commit changes**.

En **menos de un minuto**, la web mostrará esos archivos con un botón
**Descargar**. No hay que tocar nada más.

Para el otro curso, repites entrando a `material/macroeconometria`.

---

## Preguntas frecuentes

**¿Qué tipos de archivo puedo subir?**
Cualquiera: PDF, PPT/PPTX, Word, Excel/CSV, ZIP, scripts de R (`.R`), Stata
(`.do`), Python (`.py`, `.ipynb`), imágenes, etc. La web les pone un ícono de
color según el tipo.

**¿Hay límite de tamaño?**
GitHub recomienda archivos de hasta 25 MB por la web (100 MB máximo). Para datos
o videos muy pesados, mejor sube un enlace (por ejemplo a Drive) en un archivo
de texto, o comprime en ZIP.

**¿Puedo agregar un tercer curso más adelante?**
Sí. Abre `index.html`, busca la sección `COURSES` al inicio y copia un bloque
de curso siguiendo el mismo formato. Crea también su carpeta dentro de
`material/`. Si quieres, te ayudo a hacerlo.

**¿Y si uso un dominio propio (dominio UNAB)?**
En `index.html`, al inicio, cambia `REPO_MANUAL: null` por
`REPO_MANUAL: { owner: "TU-USUARIO", repo: "escuela-invierno-ipe" }`.

**La web dice "GitHub limitó las consultas".**
Es un límite de GitHub para visitas anónimas muy seguidas (60 por hora por
conexión). Se soluciona solo esperando unos minutos. Para un curso normal no
debería aparecer.
