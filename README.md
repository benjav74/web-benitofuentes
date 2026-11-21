# benitofuentes.com · prototipo v2

Sitio estático (HTML + CSS, sin JavaScript ni dependencias). Se despliega en Vercel tal cual: framework «Other», sin comando de build, directorio de salida la raíz.

- `index.html`: portada con datos estructurados JSON-LD (ProfilePage, Person, WebSite, OfferCatalog con 4 Service).
- `aviso-legal.html`, `privacidad.html`: pendientes de texto legal.
- `robots.txt`, `sitemap.xml`, `llms.txt`, `404.html`, `vercel.json` (URLs limpias, cabeceras, caché y redirecciones desde las URLs antiguas de WordPress).
- Fuentes autoalojadas en `fonts/` (Montserrat, Open Sans y Fjalla One, las de la web actual).

Publicación de prueba en un dominio *.vercel.app: `vercel.json` envía `X-Robots-Tag: noindex` en todas las rutas y `robots.txt` es `Disallow: /`. Al pasar el dominio a benitofuentes.com, quitar esa cabecera y restaurar `robots.txt`. El original permite todo e indica el sitemap:

```
User-agent: *
Allow: /

Sitemap: https://benitofuentes.com/sitemap.xml
```

Lo marcado como [PENDIENTE] o [VALIDAR] no se publica sin el OK de Benito.
