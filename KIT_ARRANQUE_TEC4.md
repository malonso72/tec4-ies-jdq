# Kit de arranque · Tecnología 4º ESO (tec4-ies-jdq)

Última actualización: septiembre 2026
Mantenedor: Manuel Alonso Herrera (malonso72@gmail.com)
Repositorio: github.com/malonso72/tec4-ies-jdq
Web en vivo: https://tec4-ies-jdq.malonso72.workers.dev

---

## Quién soy y qué hago aquí

- Profesor de Tecnología en el IES Jiménez de Quesada (Santa Fe, Granada).
- Esta es la web docente del curso **Tecnología · 4º ESO**.
- Cloudflare Workers (Static Assets). `git push` a `main` despliega solo (integración con GitHub); el hook de pre-push verifica HTML y enlaces antes.

## Las 8 unidades del curso

Basadas en el libro Casals adaptadas al currículo TECI II → 4º ESO, más una U0 propia:

- `00-dibujo-tecnico` — Dibujo técnico (vistas, escalas, acotación, isométrica), con 6 interactivos y 2 láminas

- `01-vivienda-sostenibilidad` — Vivienda y sostenibilidad
- `02-energias-renovables` — Energías renovables
- `03-fabricacion-diseno` — Fabricación y diseño
- `04-impresion-3d` — Impresión 3D
- `05-electronica` — Electrónica (incluye Karnaugh)
- `06-neumatica-hidraulica` — Neumática e hidráulica
- `07-robotica` — Robótica y control

## Otros repos que llevo

Si te pido tocar algo de OTRO curso, no es este repo. Dilo y abrimos otro chat.

- `tyd2-ies-jdq` — Tecnología y Digitalización · 2º ESO (tiene KIT_ARRANQUE_TYD2.md)
- `tyd3-ies-jdq` — Tecnología y Digitalización · 3º ESO (tiene KIT_ARRANQUE_TYD3.md)
- `cyr1-ies-jdq` — Computación y Robótica · 1º ESO
- `teci2-ies-jdq` — Tecnología e Ingeniería II · 2º Bachillerato (tiene KIT_ARRANQUE_TECI.md)
- `tecnologia-ies-jdq` — hub general

## Tono y forma de trabajar

- Español, conciso, sin verborrea.
- No uses emojis salvo que yo los use primero.
- Cambio en varios pasos → primero RECAP de lo entendido y espera mi OK antes de tocar nada.
- Cambio claro y autocontenido → hazlo y resumes al final.
- El push lo decido yo: tú haces commit y me preguntas antes de hacer push (despliega a la web que usan los alumnos).
- A veces se cuelga `.git/index.lock` y bloquea commits desde GitHub Desktop. Hay que borrarlo del disco.
- Antes de cambios grandes deja backup con sufijo `.bak_<descripcion>`.

## Decisiones que NO hay que rediscutir

### Estructura del libro digital de cada unidad

Mismo patrón que el resto de mis webs:
- `unidades/0X-nombre/libro-digital.html` con `const banco = { 1: {...}, ..., N: {...} }` y `const imgs = {...}`.
- LaTeX MathJax con `\\[ ... \\]` en `teoria_html`.
- Imágenes EMBEBIDAS como data URLs.
- Esquemas vectoriales → SVG inline con `width` y `height` EXPLÍCITOS y subíndices con `<tspan>`.

### Contenidos específicos de 4º

- U5 Electrónica incluye **mapas de Karnaugh** (no aparece en 2º ni 3º).
- U6 Neumática e hidráulica es contenido NUEVO de este curso.
- U7 Robótica es continuación de la de 3º pero con más profundidad de programación y sensores.

### Exámenes (cuando te pida uno)

Esquema por defecto:
- Word `.docx` para alumno + solucionario aparte.
- Cabecera con datos del alumno + caja "NOTA __/10".
- **Teoría tipo test**, 4 opciones, cuadradito ☐ delante. Sin penalización.
- **Ejercicios** con cálculos, espacio en blanco con borde inferior.
- Solucionario en VERDE con paso a paso.

## Estado (septiembre 2026)

Las 8 unidades tienen hub, libro digital, interactivos, actividades, autocomprobación y proyecto
(U0: actividades y proyecto pendientes). Auditoría completa hecha en septiembre de 2026; lo ya
corregido y lo que queda está en `documentacion/PENDIENTES.md`.

Convenciones fijadas en esa auditoría:
- Mapas de Karnaugh: columnas **ab**, filas **c**/**cd** en Gray (la disposición de clase y del simulador D2 de TECI II). No adaptar a la del libro de texto.
- Símbolos neumáticos: ISO 1219-1, generados desde `simbolos.py` (fuente en el chat de la auditoría); los orificios de una distribuidora se dibujan sobre el cuadrado de reposo, el del lado del muelle.
- Los tests de autocomprobación tienen las opciones equilibradas en longitud: al añadir preguntas, la correcta no debe ser la más larga.
- El libro es material de apoyo: no ampliar texto; sí figuras donde el contenido es visual.

## Cómo arrancar conmigo

Lee este kit y `CLAUDE.md`, confirma «listo» y espera la tarea. Si la tarea no es de este repo (Tecnología 4º ESO), avisa para abrir un chat separado.
