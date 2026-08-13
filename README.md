# Centro Internacional de Ciencias A.C. — Sitio Web Institucional

**URL en producción:** https://cicc.org.mx/ (dominio propio, Cloudflare Pages) — respaldo: https://intro117.github.io/cicc/  
**Repositorio:** github.com/intro117/cicc  
**Rama activa:** `main` (deploy automático vía Cloudflare Pages en cada push; GitHub Pages se mantiene activo como respaldo)

---

## Descripción general

Rediseño completo del sitio institucional del **Centro Internacional de Ciencias A.C. (CIC)**, fundado en 1986 en Cuernavaca, Morelos, México. El sitio reemplaza la versión original construida con Netscape Composer en 1999 (`cicc.unam.mx`) por una página moderna, responsiva, accesible y con animaciones 3D interactivas.

Todo el contenido fue extraído y verificado directamente del sitio oficial existente en `http://www.cicc.unam.mx/` y sus subpáginas.

---

## Estructura del repositorio

```
cicc/
├── index.html                          ← SITIO PRINCIPAL (versión final integrada)
├── LOGO_-_Centro_Internacional_de_Ciencias_NEGRO__1_.png
├── README.md
├── propuesta1/
│   ├── index.html                      ← Variante A: Azul Noche + Oro académico
│   └── LOGO_-_...png
├── propuesta2/
│   ├── index.html                      ← Variante B: Azul Petróleo + Aqua (base del sitio final)
│   └── LOGO_-_...png
└── propuesta3/
    ├── index.html                      ← Variante C: Azul Institucional + Ocre dorado
    └── LOGO_-_...png
```

> Las carpetas `propuesta1/`, `propuesta2/` y `propuesta3/` se conservan como respaldo histórico de las variantes de diseño presentadas al cliente. El sitio en producción es el `index.html` de la raíz.

---

## Tecnologías utilizadas

| Tecnología | Versión / Fuente | Uso |
|---|---|---|
| HTML5 semántico | — | Estructura completa |
| CSS3 con variables custom | — | Sistema de diseño con tokens |
| JavaScript vanilla (ES5 compatible) | — | Interactividad, tabs, nav |
| Three.js | r128 (cdnjs CDN) | Animaciones 3D del Punto de Fermat |
| Google Fonts | Crimson Pro + Inter | Tipografía editorial |
| OpenStreetMap embed | — | Mapa sin API key |

Sin frameworks frontend. Sin dependencias de npm. Sin build step. Abre directamente en el navegador.

---

## Secciones del sitio (orden de aparición)

### 1. Hero — Pantalla completa con animación Three.js
- Canvas 3D con el diagrama del Punto de Fermat animado
- Partículas flotantes con los colores del logo oficial (azul `#5050f0`, rojo `#f00000`, amarillo `#f0f078`)
- Parallax con el movimiento del mouse
- Texto centrado: nombre institucional + tagline
- **Fuente:** identidad visual del CIC / logo oficial

### 2. El CIC y el Punto de Fermat (`#acerca`)
- Canvas 3D interactivo del logo (drag to rotate, touch habilitado)
- Explicación editorial numerada en 4 pasos de la construcción geométrica
- Misión oficial integrada como cita destacada
- Cifras institucionales: 1986, 37 asociados, 4 instituciones, 28+ años
- **Fuente verificada:** `http://www.cicc.unam.mx/mission.html`

### 3. Nosotros (`#nosotros`)
- **Misión:** texto extraído y adaptado de `mission.html`
- **Visión:** redactada a partir del contexto institucional verificado
- **Valores:** Interdisciplina, Apertura, Colaboración, Rigor científico (inferidos de la filosofía del CIC)
- **Historia / línea de tiempo:** 1986 (fundación), 1998 (inicio archivo digital), 2000s (expansión temática), 2021 (adaptación digital), hoy
- **Cuernavaca:** texto adaptado de `http://www.cicc.unam.mx/cuernavaca.html` — descripción geográfica, clima, densidad de doctores por habitante

### 4. Actividades académicas (`#actividades`)
Todas las fechas y actividades son verificadas directamente del sitio oficial.

#### Actividades 2026 (estado: finalizadas al 12 ago 2026)
| Fecha | Actividad | Fuente |
|---|---|---|
| 5–9 enero 2026 | Taller de Nanosistemas III | `activities/2026/QTech/` |
| 12 mayo 2026 | Reunión Anual División Estado Sólido SMF | `des-smf.mx` |

**Fuente:** `http://www.cicc.unam.mx/activities/2026/index.html`

#### Archivo histórico con tabs (2025–2021)

**2025** — `activities/2025/index.html`
- Reunión Anual División Estado Sólido SMF (5–7 mayo)
- Taller de Nanosistemas I (24–28 noviembre)
- Taller de Nanosistemas II (9–13 diciembre)

**2024** — `activities/2024/index.html` (verificado mediante scraping)
- Econofísica y Econometría en Finanzas (15–19 julio)
- Mini-Conferencia Finanzas y Econofísica (19–20 julio)
- Random Matrix Theory y sus aplicaciones (22–26 julio)
- From Quasi-2D Systems to Molecular Devices (26 ago–5 sep)

**2023** — `activities/2023/index.html`
- Multivariate Analysis in Finance, Brain Research (23–28 abril)
- Taller Germi Beta Fest (16–17 junio)
- Gathering de Ondas y Materiales GOMA (25 jun–1 jul)
- Escuela de Verano: IA y Análisis de Datos (3–14 julio)
- Transport at the Nanoscale (6–10 noviembre)
- Econometrics, Econophysics and Transport (21–25 noviembre)

**2022** — `activities/2022/index.html`
- Multivariate Analysis in Finance and Brain Research (7–11 febrero)
- Symposium: Quantum and Classical Dynamics / RMT (28 feb–4 mar)
- Escuela: Análisis de Series de Tiempo e IA (30 mayo–10 jun)
- Indo-Mexican Workshop: Multivariate Analysis & ML (13–24 junio)
- GOMA: Dinámica de Ondas en Sistemas Complejos (30 oct–4 nov)
- Transport at the Nanoscale (5 noviembre)

**2021** — `activities/2021/index.html`
- UdG-UV-UNAM-BUAP: Open Systems & Quantum Dynamics (5–15 enero)
- Classical and Quantum Dynamics of Complex Systems (22 mar–1 abr)
- Coarse graining and fuzzy measurements (18–20 agosto)
- Mini-workshop: Multivariate Analysis (8 octubre)
- Congreso de Ondas, Materiales y Metamateriales (21–26 noviembre)

#### Panel "Todos los años" — 22 años académicos enlazados
Links directos a todos los índices desde 1998–1999 hasta 2020, extraídos del índice oficial `http://www.cicc.unam.mx/activities/`.

### 5. Comunidad científica (`#comunidad`)
**Fuente verificada:** `http://www.cicc.unam.mx/associate.html`

**Directivos:**
- Dr. Adán Oswaldo Guerrero Cárdenas — Director
- Dr. François Alain Leyvraz Waltz — Presidente (ICF UNAM)
- Dr. Thomas Henry Seligman Schurch — Presidente de la Asamblea (ICF UNAM)

**Miembros asociados mexicanos (selección de 30+ verificados):**
Dr. Gustavo Martínez Mekler, Dr. Luis Mochán Backal, Dr. Alberto Darszon, Dr. Kurt Bernardo Wolf, Dr. Antonio Lazcano Araujo, Dr. Alejandro Frank, Dr. Luis Montejano, Dr. Thomas Gorin — entre otros.

**Miembros internacionales (verificados):**
- Dr. Anirban Chakraborti — Jawaharlal Nehru University, India
- Dr. Thomas Guhr — Univ. Duisburg-Essen, Alemania
- Dr. Vladimir Y. Man´ko — Lebedev Institute, Rusia
- Dr. Itamar Procaccia — Weizmann Institute, Israel
- Dr. Tomaz Prosen — Univ. Ljubljana, Eslovenia
- Dr. Hans A. Weidenmüller — Max-Planck-Institut, Alemania

**Instituciones miembro (verificadas):**
- Academia Mexicana de Ciencias (AMC)
- Universidad Autónoma del Estado de Morelos (UAEM)
- Universidad Nacional Autónoma de México (UNAM)
- Coordinación de la Investigación Científica, UNAM

### 6. Visitantes de largo plazo y Recursos (`#visitantes`)
**Fuente verificada:** `http://www.cicc.unam.mx/visitors.html`

**Investigadores en residencia (historial verificado):**
- Tania Arely Pérez Muñoz (julio 2024 en adelante)
- Dr. Alexander M. Fedotov (noviembre 2021 en adelante)
- Dr. Christian Schubert (noviembre 2021 en adelante)
- Dr. Hirdesh K. Pharasi (abril 2021 en adelante)
- Dra. Suchetana Sadhukhan (marzo 2021 en adelante)
- Marianna Euler / Norbert Euler (mayo 2019 en adelante)

**Recursos institucionales** — **Fuente:** `http://www.cicc.unam.mx/links.html`
- Instituciones UNAM: Centro de Ciencias Físicas, IB UNAM, Instituto de Matemáticas, IIMAS, Biblioteca UNAM
- Revistas: arXiv, Physical Review Letters, Physica A (Elsevier), JNMP
- Centros aliados: ICTP Trieste, Max Planck Dresden, ACMOR, CIE UNAM

### 7. Contacto (`#contacto`)
**Fuente verificada:** `http://www.cicc.unam.mx/` (tabla de contacto) + `cuernavaca.html`

- Dirección: Av. Universidad 1001, Campus UAEM-UNAM, Col. Chamilpa, CP 62210, Cuernavaca, Morelos
- Teléfono institucional: +52 (777) 329-1877
- WhatsApp administración: +52 777 650 0712
- Correo: cicadmon1@gmail.com
- Facebook: Centro Internacional de Ciencias
- Mapa embebido: OpenStreetMap (sin API key)
- Instrucciones llegada desde CDMX: autobuses Pullman de Morelos (~90 min)

---

## Sistema de diseño

### Paleta de colores
| Token CSS | Valor HEX | Uso |
|---|---|---|
| `--bg-osc` | `#1b3a4b` | Fondo oscuro principal |
| `--bg-osc2` | `#142e3d` | Fondo oscuro profundo |
| `--bg-osc3` | `#0f2535` | Fondo más profundo / footer |
| `--bg-cla` | `#ffffff` | Secciones claras |
| `--bg-cla2` | `#f0fafa` | Fondo aqua tenue |
| `--aqua` | `#7ec8c8` | Acento principal |
| `--aqua-cl` | `#a8dede` | Aqua claro (hover) |
| `--aqua-os` | `#2a7a7a` | Aqua oscuro (fondos claros, WCAG AA) |

Los colores del logo original (azul `#5050f0`, rojo `#f00000`, amarillo `#f0f078`) se usan **exclusivamente en las animaciones Three.js** para mantener la identidad del símbolo.

### Tipografía
- **Títulos:** Crimson Pro (Google Fonts) — serif editorial, peso 300/400/600
- **Cuerpo:** Inter (Google Fonts) — sans-serif de alta legibilidad, peso 300/400/500/600

### Contraste (WCAG AA verificado)
- Texto sobre fondos oscuros: mínimo 5:1 (tokens `--txt-osc-1` a `--txt-osc-4`)
- Texto sobre fondos claros: mínimo 4.5:1 (tokens `--txt-cla-1` a `--txt-cla-5`)
- Aqua oscuro (`#2a7a7a`) sobre blanco: ratio 4.6:1 ✓

### Breakpoints
| Ancho | Cambio principal |
|---|---|
| `≤900px` | Grids pasan a 1 columna |
| `≤768px` | Nav colapsada en hamburger |
| `≤480px` | Botones en columna, stats en 2 col |

---

## Animaciones Three.js

> **⚠️ INTOCABLE:** Las dos animaciones 3D son el elemento de identidad aprobado por el cliente. No modificar bajo ninguna circunstancia.

### Hero Canvas (`#hero-canvas`)
- Diagrama del Punto de Fermat con 3 vértices azules, punto central rojo pulsante, puntos externos amarillos
- 1200 partículas flotantes (600 en móvil) con los colores del logo
- 3 aros circulares semitransparentes (los círculos circunscritos)
- Rotación lenta automática + parallax con el mouse
- `prefers-reduced-motion`: animación deshabilitada cuando el usuario lo solicita
- `IntersectionObserver`: pausa cuando el canvas no es visible

### Logo Canvas (`#logo-canvas`)
- Diagrama Fermat en 3D con materiales Phong (brillos, sombras)
- Luces: ambient + directional + 2 point lights (rojo y azul)
- Drag to rotate (mouse y touch)
- Inercia y deceleración suave al soltar
- Pulso del punto central rojo sincronizado con light intensity

---

## Accesibilidad

- Skip link visible al recibir foco (`Saltar al contenido principal`)
- `focus-visible` con outline aqua en todos los elementos interactivos
- Tabs del archivo histórico con `role="tablist"`, `aria-selected`, `aria-controls`
- `aria-label` en todos los botones sin texto visible
- `aria-hidden="true"` en todos los SVG decorativos
- `role="img"` + `aria-label` descriptivo en los canvas Three.js
- Canvas accesible con descripción textual alternativa en la sección Fermat
- Menú móvil con `aria-expanded` y cierre por `Escape`
- `prefers-reduced-motion` desactiva todas las animaciones

---

## SEO y metadatos

```html
<title>Centro Internacional de Ciencias A.C. — Cuernavaca, México</title>
<meta name="description" content="...">
<link rel="canonical" href="http://www.cicc.unam.mx/">
<meta property="og:*"> <!-- Open Graph completo -->
<meta name="twitter:card" content="summary_large_image">
```

Schema.org JSON-LD:
```json
{
  "@type": "ResearchOrganization",
  "name": "Centro Internacional de Ciencias A.C.",
  "foundingDate": "1986",
  "address": { "addressLocality": "Cuernavaca", "addressCountry": "MX" }
}
```

---

## Cómo actualizar el sitio

### Requisitos
- Git instalado en WSL2
- Acceso al repositorio `github.com/intro117/cicc`

### Flujo estándar
```bash
cd ~/cicc

# Copiar el nuevo index.html desde Descargas
cp "/mnt/c/Users/lenovo/Downloads/index.html" index.html

# Si también hay logo nuevo:
cp "/mnt/c/Users/lenovo/Downloads/LOGO_-_Centro_Internacional_de_Ciencias_NEGRO__1_.png" .

# Publicar
git add .
git commit -m "descripción del cambio"
git push
```

GitHub Pages publica automáticamente en ~60 segundos en: https://intro117.github.io/cicc/

### Actualizar actividades
Editar la sección `#actividades` en `index.html`. Los paneles del archivo histórico tienen estructura repetible:

```html
<div class="ev-card rv">
  <span class="ev-tipo t-tall">Taller</span>
  <div class="ev-fecha">DD mes – DD mes AAAA</div>
  <div class="ev-titulo">Título del evento</div>
  <a href="URL_del_evento" class="ev-link" target="_blank" rel="noopener">Ver detalles →</a>
</div>
```

Tipos disponibles: `t-conf` (conferencia), `t-tall` (taller), `t-esc` (escuela), `t-gath` (gathering), `t-sim` (simposio).

### Cambiar estado de actividades 2026
- **Próxima:** cambiar `.act-estado-fin` por clase `.act-estado-prox` y texto "Próximo"
- **Finalizado:** clase actual `.act-estado-fin` con texto "Finalizado"

---

## Pendientes del cliente

- [ ] Fotografías de Dr. Guerrero, Dr. Leyvraz y Dr. Seligman (para tarjetas de directivos)
- [ ] Fotografías de instalaciones del CIC
- [ ] Logotipos oficiales: AMC, UAEM, UNAM, Coordinación CIC
- [ ] Usuario de Instagram (si aplica)
- [ ] Actividades confirmadas del año académico 2027
- [x] Decisión sobre dominio definitivo: `cicc.org.mx` adquirido, sitio publicado vía Cloudflare Pages

---

## Fuentes de contenido verificadas

Todas las páginas del sitio `http://www.cicc.unam.mx/` que fueron consultadas y de las que se extrajo contenido:

| Página | Contenido extraído |
|---|---|
| `/` | Descripción institucional, dirección, teléfono, secciones del sitio |
| `/mission.html` | Definición del Punto de Fermat, misión oficial del CIC |
| `/associate.html` | Directivos, 30+ miembros mexicanos, 6 internacionales, 4 instituciones |
| `/visitors.html` | 6 investigadores en residencia con fechas verificadas |
| `/cuernavaca.html` | Descripción geográfica y cultural de Cuernavaca |
| `/links.html` | Instituciones UNAM, revistas científicas, centros aliados |
| `/activities/` | Índice de los 28 años académicos (1998–2026) |
| `/activities/2026/index.html` | 2 actividades verificadas |
| `/activities/2025/index.html` | 3 actividades verificadas |
| `/activities/2024/index.html` | 4 actividades verificadas |
| `/activities/2023/index.html` | 6 actividades verificadas |
| `/activities/2022/index.html` | 6 actividades verificadas |
| `/activities/2021/index.html` | 5 actividades verificadas |
| `/activities/2021/udg_buap_unam_2021/gathering1.html` | Detalle gathering enero 2021 |
| `/curricula/index.html` | Currículos de visitantes de largo plazo |

---

## Historial de versiones

| Versión | Fecha | Descripción |
|---|---|---|
| v1.0 | 5 ago 2026 | Primera versión publicada en GitHub Pages |
| v1.1 | 6 ago 2026 | Regeneración completa del index (2659 líneas) |
| v2.0 | 10 ago 2026 | 3 propuestas de diseño publicadas en subdirectorios |
| v2.1 | 12 ago 2026 | Propuesta 2 con cambios del cliente (hero, Fermat, Biotecnología-style) |
| v3.0 | 12 ago 2026 | Reestructuración: contraste WCAG, Fermat editorial, 2025/2022, miembros reales |
| v3.1 | 12 ago 2026 | Integración completa: sección Nosotros, visitantes, recursos, 2021, todos los años |
| **v4.0** | **12 ago 2026** | **Sitio final: index raíz unificado. Propuestas conservadas como respaldo.** |

---

## Créditos

**Desarrollo:** Rediseño web para Centro Internacional de Ciencias A.C.  
**Contenido:** Extraído y verificado de `http://www.cicc.unam.mx/`  
**Institución:** Centro Internacional de Ciencias A.C., Cuernavaca, Morelos, México  
**Año de fundación:** 1986  
**Contacto institucional:** cicadmon1@gmail.com · +52 777 650 0712

---

*© Centro Internacional de Ciencias A.C. Todos los derechos reservados.*

