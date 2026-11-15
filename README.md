# Áurea Seguros — sitio optimizado para SEO y AEO

Sitio en vivo: https://aureaseguros.com.mx

Reto: hackathon SEO + AEO de Hostinger / Irremplazables (noviembre 2026).

Negocio: asesoría en seguros (daños y personas para empresas, personas y familias; microseguros; seguros de arte). Herencia familiar desde 1939. Áurea Seguros es el nombre de la futura persona moral de Esquino Seguros y Fianzas; la marca está en trámite ante el IMPI.

## Qué contiene este repositorio
- `snapshot/`: copia de lo publicado, actualizada el 15-nov-2026 tras el último cambio (`robots.txt`, `sitemap.xml`, `llms.txt` y un extracto del HTML renderizado). Es una copia de consulta; el sitio se construyó y se publica con Hostinger AI Builder, que no exporta el código fuente.
- `jsonld.json`: los cuatro bloques JSON-LD de la página principal (WebSite, Organization, InsuranceAgency, FAQPage).
- `prompts/`: mensajes enviados al builder.
- `evidencia/`: capturas de compra, Lighthouse y AI Visibility.

## SEO (verificado en el sitio en vivo)
- Título de 52 caracteres y meta descripción de 156.
- Un solo H1; las preguntas del FAQ son H2 en forma de pregunta; los H3 se usan solo bajo "Nuestra asesoría".
- Canonical, etiquetas Open Graph y Twitter, `lang="es-MX"`, HTTPS.
- `sitemap.xml` con cinco URL (inicio, `/nosotros`, `/contacto`, `/privacidad`, `/terminos`) y `lastmod`; `robots.txt` publicado.
- Páginas `/nosotros` y `/contacto` con título, descripción y canonical propios; versión en Markdown de la página principal en `/home.md`.

## AEO (verificado en el sitio en vivo)
- Párrafo introductorio que dice quién es el negocio y a quién atiende.
- FAQ visible de 8 preguntas; la primera oración de cada respuesta da el dato.
- JSON-LD InsuranceAgency, Organization y FAQPage (más AboutPage, ContactPage y BreadcrumbList en las páginas internas) con el mismo texto que la página.
- Fecha de última actualización visible en el pie ("Última actualización: 15 de noviembre de 2026.").
- Contenido presente en el HTML inicial, sin depender de JavaScript para leerlo.
- `llms.txt` publicado. Es un complemento: Google Search no lo usa.
- Datos de contacto, horario y zona en texto visible y en JSON-LD.

## Limitaciones conocidas
- `robots.txt` lo administra la plataforma y no es editable. Permite los bots de búsqueda e IA de consulta y bloquea los de entrenamiento (GPTBot, ClaudeBot, Google-Extended, entre otros).
- Search Console, Google Business Profile y perfiles en redes aún no están configurados.
- Aviso de privacidad y términos de uso publicados en `/privacidad` y `/terminos`. Son una versión básica, pendiente de revisión por una persona con formación jurídica; el aviso no incluye todos los elementos que exige la ley.
- No se afirma autorización de la CNSF para Áurea, porque la persona moral aún no está constituida. El sitio dice que las pólizas las emiten aseguradoras autorizadas y supervisadas por la CNSF.
- No se garantizan resultados de posicionamiento ni de aparición en respuestas de IA.
