# Formless Studio — Brand README
> Tipografías, paleta de colores e identidad visual del estudio.

---

## Tipografías

### 01 · Space Grotesk — Cuerpo principal

Fuente moderna y geométrica con un toque técnico. Se usa para títulos grandes, párrafos, subtítulos y cualquier texto de lectura.

- **Pesos usados:** 300 (light), 400 (regular), 600 (semibold), 700 (bold)
- **Dónde conseguirla:**
  - Google Fonts → https://fonts.google.com/specimen/Space+Grotesk
  - Importar en CSS: `@import url('https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@300;400;600;700&display=swap');`
  - Descargar para uso local: en Google Fonts, botón **"Download family"**

---

### 02 · Space Mono — Etiquetas, nav y código

Fuente monoespaciada de la misma familia. Refuerza la identidad del estudio con una estética técnica/terminal. Se usa para navegación, etiquetas, CTAs, precios y badges.

- **Pesos usados:** 400 (regular), 700 (bold)
- **Dónde conseguirla:**
  - Google Fonts → https://fonts.google.com/specimen/Space+Mono
  - Importar en CSS: `@import url('https://fonts.googleapis.com/css2?family=Space+Mono:wght@400;700&display=swap');`
  - Descargar para uso local: en Google Fonts, botón **"Download family"**

---

### Importar ambas juntas (recomendado)

```css
@import url('https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@300;400;600;700&family=Space+Mono:wght@400;700&display=swap');
```

```css
/* Variables CSS */
--font-main: 'Space Grotesk', sans-serif;
--font-mono: 'Space Mono', monospace;
```

---

## Paleta de colores

### Colores primarios

| Nombre | HEX | Uso |
|---|---|---|
| Lima / Brand | `#C8F135` | Acento principal, CTAs, íconos, highlights |
| Negro base | `#111111` | Fondo principal de todas las páginas |
| Negro medio | `#1E1E1E` | Cards, paneles, superficies secundarias |

---

### Colores de texto

| Nombre | HEX | Uso |
|---|---|---|
| Blanco principal | `#FFFFFF` | Títulos y headings principales |
| Gris claro | `#E8E8E8` | Cuerpo de texto general |
| Gris muted | `#888888` | Texto secundario, descripciones, labels |
| Negro | `#111111` | Texto sobre fondo lima (ej. botones CTA) |

---

### Colores de borde y UI

| Nombre | HEX / Valor | Uso |
|---|---|---|
| Border lima | `rgba(200, 241, 53, 0.2)` | Bordes de cards, separadores, grids |
| Border hover | `rgba(200, 241, 53, 0.4)` | Estados hover / destacados |
| Overlay grid | `rgba(200, 241, 53, 0.04)` | Patrón de cuadrícula de fondo (hero) |

---

### Paleta completa resumida

```
#C8F135   ████  Lima Brand
#111111   ████  Negro Base
#1E1E1E   ████  Negro Medio
#FFFFFF   ████  Blanco
#E8E8E8   ████  Gris Claro
#888888   ████  Gris Muted
```

---

## Reglas de uso

- El lima `#C8F135` **nunca** va sobre fondo blanco — solo sobre negro/oscuro.
- El texto sobre fondo lima siempre es `#111111` (negro puro).
- No mezclar más colores de acento — la identidad descansa en el contraste lima/negro.
- El patrón de cuadrícula en el hero es opcional pero refuerza la estética Minecraft sin ser literal.

---

## Fuentes — alternativas offline

Si no tienes acceso a Google Fonts en producción, puedes descargar los archivos `.ttf` o `.woff2` directamente desde:

- **Fontsource (npm):** `npm install @fontsource/space-grotesk @fontsource/space-mono`
- **GitHub de las fuentes:**
  - Space Grotesk → https://github.com/floriankarsten/space-grotesk
  - Space Mono → https://github.com/googlefonts/spacemono

---

## Iconos

### Librería usada: Tabler Icons

Set de íconos outline (trazo, sin relleno) — coherente con la estética técnica y limpia del estudio.

- **Sitio oficial / buscador:** https://tabler.io/icons
- **Cantidad:** 5800+ íconos disponibles
- **Estilo usado:** outline únicamente (nunca `-filled`)

---

### Cómo usarlos en web (webfont — método del diseño)

```html
<!-- Cargar la fuente una sola vez -->
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/@tabler/icons-webfont/dist/tabler-icons.min.css">

<!-- Usar cualquier ícono -->
<i class="ti ti-map"></i>
<i class="ti ti-building-skyscraper"></i>
<i class="ti ti-world"></i>
```

El ícono hereda el color y tamaño del elemento padre via CSS (`font-size`, `color`).

---

### Cómo encontrar el nombre de un ícono

1. Ir a https://tabler.io/icons
2. Buscar en inglés lo que necesitas (ej. `"sword"`, `"map"`, `"cube"`)
3. El nombre que aparece debajo es exactamente el que usas con prefijo `ti-`
   - Nombre en sitio: `map` → clase CSS: `ti ti-map`
   - Nombre en sitio: `brand-discord` → clase CSS: `ti ti-brand-discord`

---

### Íconos usados en el diseño

| Ícono | Clase CSS | Dónde se usa |
|---|---|---|
| Mapa | `ti ti-map` | Servicio: Mapas de aventura |
| Edificio / skyline | `ti ti-building-skyscraper` | Servicio: Spawn & Hub |
| Mundo / globo | `ti ti-world` | Servicio: Setup completo |
| Discord | `ti ti-brand-discord` | Contacto — red social |
| Email | `ti ti-mail` | Contacto — correo |
| Reloj | `ti ti-clock` | Contacto — tiempo de respuesta |
| Check | `ti ti-check` | Sección valores / lista |

---

### Instalación alternativa (npm para proyectos)

```bash
npm install @tabler/icons
# o solo el webfont
npm install @tabler/icons-webfont
```

---

### Íconos útiles para Minecraft / gaming (sugeridos)

| Concepto | Clase CSS |
|---|---|
| Mapa / mundo | `ti ti-map`, `ti ti-globe` |
| Construcción | `ti ti-hammer`, `ti ti-tools` |
| Servidor | `ti ti-server` |
| Comunidad / Discord | `ti ti-brand-discord` |
| Pago / comisión | `ti ti-credit-card`, `ti ti-currency-dollar` |
| Entrega / descarga | `ti ti-download`, `ti ti-package` |
| Estrella / calidad | `ti ti-star` |
| Tiempo / plazo | `ti ti-clock`, `ti ti-calendar` |
| Configuración | `ti ti-settings` |
| Usuario / cliente | `ti ti-user` |

---

*Formless Studio — BUILDS. CONFIG. DESIGN.*