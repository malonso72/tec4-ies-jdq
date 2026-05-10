# Decisiones de diseño · Tecnología 4º ESO

Bitácora de decisiones técnicas y editoriales del proyecto.

## 2026-05-10 · Bootstrap del sitio (v1.0.0)

- **Modelo de referencia:** `teci2-ies-jdq`, `tyd2-ies-jdq` y `tyd3-ies-jdq`.
  Misma estructura modular, misma tipografía, misma filosofía vanilla.
- **Slug del repo:** `tec4-ies-jdq` (no `tyd4-ies-jdq`) porque la asignatura
  en 4º se llama "Tecnología" (no "Tecnología y Digitalización"). Decisión
  documentada en §7 del brief v1.2.0.
- **Paleta morado-violeta** (`--principal #5E3B91`). Cierra la progresión:
  1º verde-cian → 2º naranja → 3º burdeos → 4º morado. Todas diferenciables
  del azul TECI.
- **Estructura por unidades didácticas integradas** (no por bloques temáticos).
  Cada unidad tiene `index.html` + `teoria.html` + `actividades.html`.
- **Slug numerado de 2 dígitos** (`01-...` a `07-...`).
- **Enlaces cruzados (§7.3 del brief): doble dirección.**
  - **Repaso TyD3** (callout `callout-info`, icono 🔁): U3, U5, U7
  - **Profundización TECI II** (callout `callout-key`, icono 🎓): U2, U5, U6, U7
  - URLs absolutas a los subdominios Cloudflare hermanos.
  - U5 y U7 llevan los dos callouts (repaso + profundización), señalando el
    rol de bisagra: vienen de TyD3 y siguen hacia 2º Bachillerato (TECI II).
- **CSS modular** con paleta en `:root` de `common.css`.
- **Solucionarios privados** en `_soluciones/`, excluido del despliegue
  vía `.assetsignore`.

## Convenciones

- Slug de unidad: `NN-kebab-case` con dos dígitos (`01-`, `02-`, ..., `07-`).
- Commits: español, verbo en imperativo, versión al final entre corchetes.
- Sin frameworks. Sin CDNs salvo Google Fonts y MathJax.
