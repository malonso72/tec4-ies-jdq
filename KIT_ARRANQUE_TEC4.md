# Kit de arranque · Tecnología 4º ESO (tec4-ies-jdq)

Última actualización: junio 2026
Mantenedor: Manuel Alonso Herrera (malonso72@gmail.com)
Repositorio: github.com/malonso72/tec4-ies-jdq
Web en vivo: https://tec4-ies-jdq.malonso72.workers.dev

---

## Quién soy y qué hago aquí

- Profesor de Tecnología en el IES Jiménez de Quesada (Santa Fe, Granada).
- Esta es la web docente del curso **Tecnología · 4º ESO**.
- Cloudflare Workers (Static Assets). Despliegue manual con `npx wrangler deploy` desde la raíz. No hay auto-deploy desde GitHub.

## Las 7 unidades del curso

Basadas en el libro Casals adaptadas al currículo TECI II → 4º ESO:

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
- Los deploys los hago yo (`git push` + `npx wrangler deploy`); tú no tienes credenciales.
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

## Estado al cerrar este chat (junio 2026)

Repo LIMPIO. `git status` = nothing to commit. Branch `main` al día con origin.

Trabajo hecho hasta ahora en este repo:
- Las 7 unidades creadas con su estructura base.
- Mapeo de contenidos TECI II → 4º ESO documentado.
- Índice del libro Casals leído y usado de base.

Pendiente (cuando vuelvas en septiembre, no lo arranques tú solo — espera mi tarea):
- Posibles ampliaciones por unidad según vea en clase.
- Posibles exámenes por unidad con el formato test + ejercicios.
- Interactivos o microactividades si surgen.

## Cómo arrancar conmigo en septiembre

Cuando vuelva, espera a que te diga la tarea. No audites el repo ni propongas cosas por tu cuenta. Solo:

1. Lee este kit.
2. Confirma "listo, todo cargado" y queda a la espera.
3. Yo te indico la tarea concreta.

Si la tarea no es de este repo (Tecnología 4º ESO), avisa para abrir un chat separado para el repo correspondiente.
