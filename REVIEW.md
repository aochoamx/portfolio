# Revisión del portafolio — forma y fondo

Fecha: 2026-09-16 · Sitio: https://portfoliosf.aochoamx.workers.dev/ · Archivos: `index.html`, `styles.css`, `Antonio-Ochoa-CV.pdf`

## Veredicto en una línea

La **forma** ya está al 80 %: diseño coherente, jerarquía clara, buen OG/social, sin errores de consola. El **fondo** está al 55 %: hay inconsistencias de datos que un reclutador detecta en segundos, los proyectos describen retos pero no resultados, y faltan señales que los filtros de contratación buscan (educación, metodologías, disponibilidad, resultados cuantificados).

## Lo que ya funciona (no lo toques)

- Paleta, tipografía (Sora + Inter) y tarjetas: se ve profesional y moderno.
- Certificaciones con enlace a Credly y número de credencial PMP (`index.html:423-438`). Esto es verificable y da confianza.
- Meta tags completos: title, description, canonical, Open Graph, Twitter card, favicon SVG + PNG + Apple touch (`index.html:6-27`).
- Cero errores de consola en producción; sin overflow horizontal en 375 px; el menú hamburguesa abre y cierra.
- Cifras de impacto en "Value I deliver": 33 % de reducción de gastos y 40 % en proveedores (`index.html:158`). Este es el tipo de dato que hay que replicar en cada proyecto.

---

# FONDO (contenido, posicionamiento, credibilidad)

## 1. Inconsistencias de datos — arreglar hoy

| Dónde | Dice | Problema |
|---|---|---|
| `index.html:71` y `:136` | "11 years leading IT & Telecom projects" | Quick Facts (`:175`) y el CV dicen "10+ years". Contando desde UANL 2014 son 12. Elige una cifra y úsala en sitio, CV y LinkedIn. |
| `index.html:90-91` | "6 Enterprise employers" | Es una métrica débil (número de empleadores no es un logro) y además el texto del hero menciona IDS (`:72`), que no aparece en el CV ni en la línea de tiempo. Sustituir por un logro: "12 terminales migradas" o "90 % de entregas a tiempo". |
| `index.html:185` | "2002–14 · Business Analyst → Developer · TATA · UANL · INFOTEC" | Cronología invertida (fuiste Developer 2002-08 y luego BA 2008-13) y UANL fue PM TI en 2014-15, no cabe en esa fila. Corregir a "Developer → Business Analyst" y dar a UANL su propia fila como PM. |
| `index.html:253` y `:276` | Logo de NTT Data junto al texto "Amazon" y "Megacable" | Visualmente se lee "logo NTT Data = Amazon". Aclarar la relación: "Amazon · via NTT Data". La tarjeta de Cinépolis (`:299`) no lleva logo, inconsistente con las otras cuatro. |
| `index.html:287` y `:310` | "migration of the new server to the cloud" en ISE y "new server migration to the cloud" en Meraki | El mismo reto en dos proyectos distintos parece copy-paste. Diferencia la historia de cada uno. |
| `index.html:216, 239, 262, 285, 308` | "2024–2025", "09 / 2025", "2026" | Tres formatos de fecha distintos. Estandariza (por ejemplo "Mar 2024 – Dic 2024"). |
| `index.html:154` | "90% project efficiency" | Métrica indefinida; un entrevistador preguntará "eficiencia de qué". Cámbiala por "% a tiempo / % dentro de presupuesto" o define la fórmula. |

**Confidencialidad:** verifica que puedes nombrar Amazon, Megacable y Cinépolis como clientes de NTT Data. Si hay NDA, usa "líder global de e-commerce", "operador telecom nacional", "cadena de cines nacional". Para un PM, respetar la confidencialidad es parte del perfil.

## 2. Hero y posicionamiento

- El titular "Turning complex IT challenges into impactful solutions through technology, innovation, and AI" (`index.html:64`) es genérico: podría ser de cualquiera. En móvil ocupa seis líneas. Propuesta de 10 palabras con dominio y prueba: *"IT & Telecom projects delivered on time and on budget — $2M+ budgets, 12-terminal rollouts, PMP + Scrum."*
- Tres roles en el hero (`:66-68`): "IT Project Manager", "Product Owner", "Technology Project Leader". El tercero es vago y diluye. Lidera con uno (IT Project Manager) y deja Product Owner como secundario.
- Falta arriba del pliegue: ubicación + modalidad + disponibilidad ("Mexico City · Remote/Hybrid · Available now"). Los reclutadores filtran por esto antes de leer nada más.
- "Diploma in Machine Learning + AI Transformation Leader course" (`:111`) sin institución. Una credencial sin emisor se descuenta a cero. Igual en la lista de certificaciones (`:445-455`), donde la columna "issuer" dice "Professional Diploma" o "AI / ML Specialization", que no son emisores.

## 3. Sección Profile

- El título "Profile built for recruiters and decision-makers" (`:132`) habla de la página, no de ti. Cámbialo por una afirmación sobre ti ("PM híbrido PMI + Agile con base técnica").
- Los dos párrafos (`:135-148`) son buenos pero largos; en móvil son dos pantallas de texto antes de llegar a los proyectos. Reduce a la mitad y mueve el detalle a las tarjetas.
- Quick Facts (`:172-179`): añade Education, Availability, Work modality, y si aplica, estatus para trabajar en EE. UU. o disposición a viajar. El silencio en estos puntos hace que te salten.

## 4. Proyectos — la sección más importante y la más incompleta

Cada tarjeta tiene Budget / Duration / Delivered / Challenge, pero **ninguna tiene Resultado**. Sin resultado, una tarjeta se lee como descripción de puesto, no como logro. Estructura recomendada por tarjeta: **Contexto → Mi rol y equipo → Qué hice → Resultado medible**.

- **SIMEX App** (`:205-225`): "Challenge solved: many stakeholders and a combined scope — aligned through a clear vision" no es un problema resuelto, es una descripción. Falta: ¿cuántos usuarios? ¿qué proceso en papel se eliminó? ¿a tiempo y en presupuesto?
- **SIMEX M&R** (`:228-248`): la mejor tarjeta técnicamente (SAP, web services, carga de datos). Falta el resultado: ¿inventario conciliado? ¿tiempo de reparación reducido?
- **Videoconferencia** (`:251-271`): buena historia de riesgo (pisos en renovación, suministro). Cierra con "12 salas entregadas en 4 meses, 0 días de retraso".
- **Cisco ISE** (`:274-294`) y **Meraki** (`:297-317`): ver duplicado arriba. Meraki es la tarjeta con más potencial "AI" real; cuéntala como caso: qué insight generaron las cámaras y qué decisión de staffing tomó el cliente.
- **Rol y tamaño de equipo ausentes** en las cinco. La seniority de un PM se juzga por presupuesto (ya está) y por headcount liderado y número de proveedores. Añade una línea "Team: 6 internos + 2 proveedores".
- **Solo 5 proyectos en 12 años de PM**, y 7 años en GMXT se resumen en dos. DUMAGO ("traer proyectos retrasados de vuelta al carril", CV) es una gran historia de PM que no aparece. Añade 2-3 proyectos más, aunque sea en una lista compacta con año y presupuesto.
- **Imágenes de stock** en las cinco. Para un PM, la prueba de trabajo es un artefacto: un Gantt anonimizado, un dashboard de Power BI, un diagrama de arquitectura. Una sola imagen real vale más que cinco de stock.
- Etiquetas (`:220-222`, etc.): "Presentations" como tag es débil; mezcla soft skills con tecnología. Separa "Skills" de "Tech".

## 5. Skills

- La tarjeta destacada (fondo oscuro) es "AI & Technology — the differentiator" (`:331-343`). Para una vacante de PM, contratan primero por entrega; la IA es el plus. Destaca "Project & Product Leadership" y deja IA en segundo lugar. Python y C# no son "AI"; muévelos a un bloque técnico.
- Metodologías (`:364-369`): solo PMI, Scrum, Agile. Los ATS buscan tokens: PMBOK 7, Hybrid/Waterfall, Kanban, Change Management, e ITIL o SAFe solo si es verdad.
- Herramientas (`:378-384`): **falta Jira/Confluence o Azure DevOps**. Casi toda vacante de PM en IT los lista; su ausencia llama la atención. "Office 365" es hoy "Microsoft 365".
- **Falta un bloque de dominio técnico** aunque aparece en los proyectos: Cisco networking, UC/videoconferencia, Cisco ISE/Meraki, SAP IM integration, AWS, mobile. Esto es lo que te diferencia de un PM genérico.
- Barras de idioma (`:406-407`): "Proficient 90 %" es decoración. Usa nivel CEFR (C1) o "Professional working proficiency", que es el término de LinkedIn.

## 6. Certificaciones y educación

- **No aparece la carrera** (Bachelor in Computer Systems Engineering, está en el CV). Para un ingeniero es una omisión grave. Añade Education con universidad y año.
- Lista secundaria (`:443-464`): pon institución y año en cada una. Considera fecha de vigencia del PMP; los reclutadores verifican que esté activo.
- Tienes en curso AWS Cloud Practitioner (objetivo 2026). Añádelo como "In progress" — conecta con las etiquetas AWS de dos proyectos y muestra crecimiento.

## 7. Contacto, CTA y footer

- "Let's talk about your next project" (`:473`) suena a freelance/consultoría. Para búsqueda de empleo: "Open to IT/Telecom Project Manager roles · Mexico City · Remote or hybrid · Available from [fecha]".
- Teléfono público (`:481`): es una decisión consciente (spam vs. reclutadores). Si lo mantienes, está bien; si notas spam, deja solo email y LinkedIn.
- Footer (`:493-494`): "Built with a human + AI workflow" enlaza a un mailto, que no tiene sentido. Además el nombre completo "Antonio Ochoa Cerón" solo aparece aquí; usa el mismo nombre que en LinkedIn en el title y el hero para que te encuentren.
- **Faltan testimonios.** Una o dos citas de recomendaciones de LinkedIn (con nombre y cargo) suben la confianza más que cualquier otra sección.

## 8. El CV descargable tiene erratas

Todo reclutador descarga el PDF. Erratas encontradas: "Proffesional" (×2), "Profitient", "proyect efficency", "anthenas", "maintainance", "realease", "latter" (por later), "to Up to date". Además el CV dice "Scrum Master – Scrum.org" mientras el sitio dice "PSM I"; el título del CV es "PMP Project Manager" y el del sitio "IT Project Manager & Product Owner"; el teléfono del CV no lleva +52. Corrige, exporta de nuevo y sube el PDF.

## 9. Idioma y mercado

El sitio es solo en inglés y el objetivo es México + EE. UU. Mantén inglés como principal, pero muchos filtros de RR. HH. en México operan en español. Opciones: una versión `/es/` con `hreflang`, o al menos un resumen en español en el hero. Añade también una línea explícita "Bilingual EN/ES" arriba; es un filtro duro en roles cross-border.

---

# FORMA (diseño, UX, móvil, técnica, código)

## 10. Móvil (verificado a 375 px en producción)

- **Navbar saturada**: el nombre se parte en dos líneas, "PROJECT PORTFOLIO" se parte en dos, el botón "Download CV" domina y el hamburguesa queda pegado al borde. Solución: ocultar `.brand-tag` bajo 560 px, botón CV solo icono o dentro del menú (`styles.css:686-713`).
- La **foto aparece después** del texto, roles, párrafo y botones: queda muy abajo del pliegue. En móvil la foto humaniza; considera reordenar el grid (`styles.css:704-705`) para mostrarla pequeña arriba.
- El titular ocupa 6 líneas en 375 px. Acortarlo resuelve fondo y forma a la vez.
- Menú: funciona, pero no cierra al pulsar un enlace ni con Escape, y el botón no tiene `aria-expanded` (`index.html:54`, `:500-504`).
- 3 elementos interactivos con altura menor a 44 px (objetivo táctil recomendado).

## 11. Rendimiento

- **Imágenes sin `width`/`height`** (12 de 12) → saltos de layout (CLS). Sin `loading="lazy"` en ninguna (todas cargan de golpe). Sin WebP/AVIF ni `srcset`.
- Peso: `project-simex-rail.jpg` 277 KB, `project-vc-rooms.jpg` 164 KB (1200×1186 mostrada a 190 px de alto), `profile-photo.jpg` 800×800 mostrada a 260 px. Convertir a WebP y redimensionar ahorra ~60-70 %. `og-card.png` 405 KB solo se usa en redes; conviértelo a JPG/WebP de ~100 KB.
- Google Fonts: 2 familias, 8 pesos, CSS externo que bloquea render (`index.html:30`). Reduce a 3-4 pesos o auto-hospeda las fuentes. El `preconnect` ya está bien.
- Sin cabeceras de caché largas para assets (revisar en Cloudflare) y sin cabeceras de seguridad básicas (`X-Content-Type-Options`, CSP simple). Riesgo bajo por ser estático, pero es un archivo `_headers` de cinco líneas.

## 12. SEO y descubribilidad

- **Sin JSON-LD `Person`** (0 ocurrencias): nombre, jobTitle, sameAs (LinkedIn, Credly), address. Es lo que Google usa para el knowledge panel.
- **`sitemap.xml` → 404** y el `robots.txt` es el default de Cloudflare (solo "content signals", sin línea `Sitemap:`).
- Sin `hreflang` ni `og:locale:alternate` (relevante si añades español).
- **Dominio `*.workers.dev`** parece URL de pruebas. Un dominio propio (antonioochoa.mx, aochoa.dev) cuesta ~USD 10-15/año, se ve profesional y es lo que va en el CV y en LinkedIn.
- Sin analítica: activa Cloudflare Web Analytics (gratis, sin cookies) para saber si los reclutadores entran y hasta dónde bajan.
- Title: añade "Mexico City" para búsqueda local.

## 13. Accesibilidad

- Solo 3 atributos ARIA en todo el documento. Falta `aria-expanded`/`aria-controls` en el toggle y un enlace "Skip to content".
- Contraste: `--text-soft: #7a8ba0` sobre blanco ronda 3.9:1, por debajo de AA (4.5:1) en textos pequeños como las etiquetas de `.project-meta` a 0.68rem (`styles.css:17`, `:508`).
- No hay estilos `:focus-visible` propios; el anillo por defecto se ve pobre sobre el hero oscuro.
- `scroll-behavior: smooth` y transformaciones hover sin `prefers-reduced-motion` (`styles.css:31`, `:112`, `:452`).
- Orden de encabezados: los `h4` de la franja AI van directo bajo el `h1` (saltan h2/h3). Menor.

## 14. Código y repositorio

- Variables de color con nombres engañosos: `--blue-500` es teal, `--cyan-400` es violeta, `--amber-400` es coral (`styles.css:9-12`). Renombra a semánticas (`--accent`, `--accent-2`, `--highlight`).
- CSS muerto: `.btn-outline` (`styles.css:129-134`) no se usa en el HTML, y la regla móvil `.nav-cta .btn-outline{display:none}` (`:702`) no afecta a nada.
- 8 `style=""` inline en el HTML (`index.html:219, 242, 265, 288, 311, 324, 406, 407`). Muévelos a clases.
- Los SVG de iconos se repiten inline (el check aparece 4 veces idéntico). Un sprite `<symbol>` reduce ruido.
- Repositorio sin `README.md`, sin `.gitignore` ni configuración de despliegue versionada. Un README de 15 líneas con "cómo desplegar" te salva en seis meses.
- El JS (`index.html:498-505`) está bien para el tamaño; añade cierre del menú al hacer clic en enlace.

---

# Plan de acción priorizado

## Hoy (1-2 h, casi todo fondo)

1. Unificar años de experiencia (sitio, CV, LinkedIn) y corregir la fila 2002-14 de la línea de tiempo.
2. Sustituir la estadística "6 employers" por un logro; quitar o justificar "IDS".
3. Aclarar los badges Amazon/Megacable/Cinépolis (y confirmar NDA).
4. Diferenciar los retos de ISE y Meraki; estandarizar el formato de fechas.
5. Añadir una línea de **Resultado** y una de **Rol + equipo** a cada proyecto.
6. Añadir Education (carrera) e institución + año en cada diploma.
7. Corregir erratas del CV, alinear título y certificación, re-exportar el PDF.
8. Reescribir el CTA para búsqueda de empleo con ubicación, modalidad y disponibilidad.

## Esta semana (forma)

9. Navbar móvil: ocultar tag, botón CV compacto, `aria-expanded`, cerrar menú al navegar.
10. Imágenes: `width`/`height`, `loading="lazy"`, WebP redimensionado.
11. JSON-LD Person, `sitemap.xml`, `robots.txt` propio con `Sitemap:`.
12. Contraste de `--text-soft`, `:focus-visible`, `prefers-reduced-motion`, skip link.
13. Limpiar CSS muerto, inline styles, renombrar variables de color.
14. Cloudflare Web Analytics y cabeceras `_headers`.
15. Dominio propio.

## Después (diferenciación)

16. Un caso de estudio "flagship" largo (SIMEX M&R o Meraki) con un artefacto real anonimizado.
17. Dos testimonios de LinkedIn con nombre y cargo.
18. Versión en español o resumen bilingüe + "Bilingual EN/ES" arriba.
19. Añadir Jira/Confluence, metodologías ATS, bloque de dominio técnico, AWS en curso.
20. 2-3 proyectos más (DUMAGO rescue, GMXT).
