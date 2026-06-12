# Tecnología 4º ESO · IES Jiménez de Quesada

**Tecnología · 4º ESO · Curso 2026-27**
Profesor: Manuel Alonso Herrera · Santa Fe (Granada)

Sitio estático servido por Cloudflare Workers Static Assets en
[tec4-ies-jdq.malonso72.workers.dev](https://tec4-ies-jdq.malonso72.workers.dev).

> **Nota sobre el slug.** El nombre del sitio es `tec4-ies-jdq` (no `tyd4-ies-jdq`)
> porque la asignatura en 4º se llama "Tecnología" (no "Tecnología y Digitalización").

## Estructura

```
tec4-ies-jdq/
├── index.html                  Hub principal con las 7 unidades
├── unidades/                   7 unidades didácticas
│   └── NN-slug/
│       ├── index.html          Hub de la unidad
│       ├── teoria.html
│       ├── actividades.html
│       └── img/
├── herramientas/
├── proyectos/
├── _soluciones/                Privado, NO se despliega
├── img/
├── assets/{css,js,templates}/
├── documentacion/              PROGRAMACION, DECISIONES, PENDIENTES
└── scripts/                    Auditoría
```

## Despliegue

```bash
python3 -m http.server 8000          # test local
python3 scripts/comprobar_enlaces.py # validación pre-push
npx wrangler deploy                  # deploy
```

## Convenciones

- HTML + CSS + JS vanilla. Sin frameworks.
- Tipografía: Barlow + Barlow Condensed + JetBrains Mono.
- Paleta: morado-violeta (`--principal #5E3B91`) con acento azul (`#1B4F8A`).
- Accesibilidad: skip-link, focus-visible, alt en imágenes, contraste AA.

## Enlaces cruzados (§7.3 del brief)

4º ESO es **bisagra hacia Bachillerato**. Cada unidad puede tener:

- **Repaso previo** (callout `info`, icono 🔁) → enlaza a TyD 3º ESO
- **Profundización futura** (callout `key`, icono 🎓) → enlaza a TECI II

Detalle:

| Unidad | Repaso TyD3 | Profundización TECI II |
|---|---|---|
| U2 Energías renovables | — | Bloque G — Tecnología Sostenible |
| U3 Fabricación y diseño | U2 Construcción de objetos | — |
| U5 Electrónica | U5 Circuitos y robótica | Bloque D2 — Electrónica Digital |
| U6 Neumática e hidráulica | — | Bloque C3 — Neumática e Hidráulica |
| U7 Robótica | U5 (parte robótica) | Bloque F — Sistemas Automáticos |

Modelo de referencia: `teci2-ies-jdq` (TECI II) y `tyd3-ies-jdq` (TyD 3º ESO).
