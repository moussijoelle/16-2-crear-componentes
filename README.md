# Crear componentes — ejercicio 16.2 (Astro)

Ejercicio del curso para practicar componentes en Astro. Saqué una galería con mis animes favoritos.

## Qué hace

En la home sale un grid con posts (hasta 20). Cada tarjeta muestra imagen, título, descripción, un trozo del contenido y la fecha. Los datos viven en `db.json`.

## Cómo probarlo

```sh
pnpm install
pnpm dev
```

Para producción:

```sh
pnpm build
pnpm preview
```

Demo: https://astro-16-2-componentes.netlify.app

## Cómo lo construí

- Página en `src/pages/index.astro`: lee `db.json` y hace un `.map` de los posts
- Componente `src/components/Post.astro`: recibe un `post` por props y pinta la tarjeta
- Tailwind para el layout (grid, tipografía, colores)
- `json-server` está en el proyecto como dependencia de desarrollo (por si hace falta servir JSON en local)

## Cómo comprobarlo

No hay tests. Con `pnpm dev` (o el enlace de Netlify) miro que salgan las tarjetas con imagen y texto, y que el grid se vea bien en móvil y escritorio.

---

Moussi Joelle · [github.com/moussijoelle](https://github.com/moussijoelle)
