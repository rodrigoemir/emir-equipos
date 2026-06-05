# emir-equipos — Landing pages de equipos Diagnóstico EMIR

Monorepo de páginas de producto. Cada equipo vive en su propia carpeta y se publica
como un sitio Netlify independiente apuntado a un subdominio.

## Estructura
```
emir-equipos/
  motostar/        -> motostar.diagnosticoemir.com   (este, el primero)
  <proximo>/       -> <proximo>.diagnosticoemir.com
  README.md
```

## Cómo agregar una nueva página (futuro)
1. Crea una carpeta nueva, ej. `keymaster-g3/`, con su `index.html`.
2. En Netlify: **Add new site → Import from Git** → mismo repo.
3. **Publish directory** = nombre de la carpeta (ej. `keymaster-g3`).
4. **Domain management → Add domain** = `keymaster-g3.diagnosticoemir.com`
   y crea el CNAME en tu DNS apuntando a la URL `*.netlify.app` de ese sitio.

Todas las páginas comparten un solo repo, pero cada subdominio es un sitio Netlify
con su propio "Publish directory".
