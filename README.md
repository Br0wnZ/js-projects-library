# 📚 Vanilla JS Library

Landing page construida con **Astro v5** y **Tailwind CSS**.  
Esta página muestra una biblioteca de 100 proyectos en Vanilla JavaScript, con soporte para modo claro/oscuro, SSR y diseño responsive.

---

## 🚀 Requisitos

- Node.js 18+ instalado
- npm o pnpm

---

## ⚡ Instalación

1. Clona este repositorio o descomprime el ZIP.
2. Instala dependencias:

```bash
npm install
```

---

## ▶️ Desarrollo

Ejecuta el servidor de desarrollo:

```bash
npm run dev
```

Abre en tu navegador: **http://localhost:4321**

---

## 🏗️ Build para producción

```bash
npm run build
npm run preview
```

Esto generará la salida optimizada en `.astro/` con **SSR habilitado**.

---

## 🌙 Modo claro/oscuro

- Se alterna con el botón en el encabezado.
- La preferencia se guarda en `localStorage`.

---

## 📂 Estructura del proyecto

```
astro-vanilla-js-library/
├── astro.config.mjs
├── package.json
├── tailwind.config.cjs
├── src/
│   ├── layouts/
│   │   └── Layout.astro
│   ├── components/
│   │   ├── Header.astro
│   │   ├── ProjectCard.astro
│   │   └── Footer.astro
│   ├── pages/
│   │   └── index.astro
│   └── projects.json
```

---

## 👨‍💻 Créditos

Hecho con ❤️ usando [Astro](https://astro.build) + [Tailwind CSS](https://tailwindcss.com).



---

## ☁️ Despliegue en Vercel

1. Instala dependencias (ya incluye `@astrojs/vercel`):

```bash
npm install
```

2. Sube tu proyecto a GitHub/GitLab/Bitbucket.

3. Ve a [Vercel](https://vercel.com/), crea un nuevo proyecto y conecta el repo.

4. Vercel detectará **Astro + SSR** automáticamente.

5. Pulsa **Deploy** y tu web estará online 🚀.
