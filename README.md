# Cotizador y generador de propuestas SoluCred

Herramienta interna del equipo comercial de SoftShop S.A. Cotiza en la reunión y genera la propuesta comercial lista para exportar en PDF.

Es un único archivo estático y autocontenido. No llama a ninguna API, no guarda nada y funciona sin conexión una vez cargado.

**En vivo:** https://fermendezmurto.github.io/cotizador-solucred/

## Publicarlo

Los archivos van en la raíz del repositorio, que es lo que GitHub Pages sirve por defecto.

En Settings, Pages, elegir Source: Deploy from a branch, rama `main` y carpeta `/ (root)`. En un par de minutos queda arriba.

## Actualizarlo

Se reemplaza `index.html` y se pushea. La URL sirve la nueva versión sola. El sello de versión que aparece en la barra superior de la herramienta indica cuál está publicada; conviene moverlo en cada cambio de precios.

## Advertencia

Este repositorio es público, así que **cualquiera con la URL puede descargar el archivo y leer la lista de precios, las bandas de descuento autorizadas al comercial y el piso de aprobación de Dirección**. El `robots.txt` y la etiqueta `noindex` evitan que aparezca en buscadores, pero no impiden el acceso directo.

Es una medida temporal mientras se estabiliza la herramienta. Cuando la versión esté cerrada, corresponde moverla a un hosting con control de acceso real (por ejemplo Cloudflare Access restringido a `@softshop.com.py`) o pasar el repositorio a privado.

## Qué hay acá

| Archivo | Qué es |
| :-- | :-- |
| `index.html` | La herramienta completa: cotizador y generador de propuestas. |
| `robots.txt` | Impide la indexación en buscadores. |
| `.nojekyll` | Le dice a GitHub Pages que sirva los archivos tal cual. |
