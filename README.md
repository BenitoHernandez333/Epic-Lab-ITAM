EPIC Lab ITAM 

Replica simplificada de la página del canal EPIC Lab ITAM, integrando HTML, CSS (Bootstrap 5.3), Git, GitHub y GitHub Pages.

1) Cumplimientos del proyecto

1.1 Bootstrap 5.3 por CDN y uso del grid (container, row, col) para responsive.
1.2 Secciones visibles: Inicio, Shorts, En directo; barra superior y barra lateral.
1.3 Recursos locales en img/ (imágenes y GIF) con enlaces funcionales.
1.4 Sin commits directos a main: trabajo en ramas e integración por Pull Requests.
1.5 Sitio publicado en GitHub Pages con index.html en la raíz.

2) Estructura final del repositorio

2.1 index.html en la raíz del repositorio.
2.2 Carpeta img/ en la raíz con: YTLogo.jpg, epicLab.jpg, VideoInicio.jpg, Short1.jpg, Directo1.gif.

3) Flujo de ramas y Pull Requests

3.1 feature/codigo → PR a main (código e imágenes).
3.2 feature/pages → PR a main (mover index.html a la raíz y ajustar rutas).
3.3 feature/readme → PR a main (documentación).
3.4 feature/evidencias → PR a main (videos responsive).

4) Comandos utilizados
4.1 Código inicial
git switch -c feature/codigo
git add -A
git commit -m "Código inicial + imágenes"
git push -u origin feature/codigo

4.2 Publicación en Pages (mover index.html a la raíz y ajustar rutas img)
git switch -c feature/pages
git mv cod/index.html index.html
# Editar index.html y reemplazar: ../img/  ->  img/
git add -A
git commit -m "Index en raíz y rutas img/"
git push -u origin feature/pages
