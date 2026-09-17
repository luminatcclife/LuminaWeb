# LUMINA Web

Sitio web de **LUMINA** (by sunny) — software a medida con diseño neurocognitivo para personas neurodivergentes (TDAH, alta sensibilidad, hiperfoco disperso) y profesionales bajo alta demanda atencional.

**Sitio en vivo:** https://luminatcclife.github.io/LuminaWeb/

Construido como un canvas de [Claude Design](https://claude.ai/design) (`.dc.html`), no HTML estático convencional.

## Estructura

| Archivo / carpeta | Contenido |
|---|---|
| `LUMINA Web.dc.html` | El sitio principal: hero, problema, servicios, proyectos, recorrido, fundamentos, proceso y contacto. |
| `LUMINA Brand & Design System.dc.html` | Sistema de marca de referencia (paleta, tipografía, componentes). |
| `support.js`, `doc-page.js` | Runtime del canvas de Claude Design — interpreta la sintaxis `x-dc` / `sc-for` / `sc-if` y los bindings `{{ }}`. |
| `hero-artifact.html`, `hero-prototype.html` | Prototipos de la fusión de dirección visual del hero (constelación de fundamentos, respiración ambiental, widget flotante), validados antes de aplicarse al sitio final. |
| `assets/`, `uploads/`, `scraps/` | Recursos e insumos del proyecto. |

## Ver el sitio en local

Como es un canvas de Claude Design, no un build de Vite/Next, basta con servirlo como archivos estáticos:

```bash
python -m http.server 8792
```

Y abrir `http://localhost:8792/LUMINA Web.dc.html` en el navegador.

## Paleta

| Token | Color |
|---|---|
| Crema (fondo) | `#F7F2EA` |
| Papel | `#FFFDF9` |
| Navy (texto/acento) | `#3F4A63` |
| Terracota | `#96562F` |
| Terracota claro | `#C99579` |
| Salvia | `#A5AD8E` |
| Dorado | `#C9AD78` |
| Rosa polvo | `#D9B5A2` |

Tipografía: **Fraunces** (display), **Manrope** (cuerpo), **JetBrains Mono** (etiquetas/datos), **Caveat** (acentos manuscritos).
