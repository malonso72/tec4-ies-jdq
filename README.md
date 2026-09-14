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
├── index.html                  Hub principal con las 8 unidades (U0-U7)
├── unidades/
│   └── NN-slug/
│       ├── index.html          Hub de la unidad (Saber/Hacer/Aplicar + recursos)
│       ├── libro-digital.html  Teoría (teoria.html redirige aquí)
│       ├── interactivos/       Simuladores y microactividades
│       ├── actividades/        Ejercicios resueltos (actividades.html redirige aquí)
│       ├── autocomprobacion/   Test de 18 preguntas con corrección
│       └── proyecto/           Proyecto de la unidad con rúbrica
├── _soluciones/                Privado, NO se despliega
├── img/
├── assets/{css,js,templates}/
├── documentacion/              PROGRAMACION, DECISIONES, PENDIENTES (no se despliega)
└── scripts/                    Verificación (HTML, enlaces) y hook de pre-push
```

## Despliegue

`git push` a `main` despliega automáticamente en Cloudflare (integración con GitHub).
El hook de pre-push ejecuta antes `scripts/verificar_html.py`, `scripts/verificar_enlaces.py`
y `scripts/comprobar_enlaces.py` y bloquea el push si algo falla.

```bash
python3 -m http.server 8000          # prueba local
python3 scripts/verificar_html.py    # HTML bien formado
python3 scripts/verificar_enlaces.py # enlaces y anclas
git push                             # despliega
```

## Convenciones

- HTML + CSS + JS vanilla. Sin frameworks.
- Tipografía: Barlow + Barlow Condensed + JetBrains Mono.
- Paleta: morado-violeta (`--principal #5E3B91`) con acento azul (`#1B4F8A`).
- Accesibilidad: skip-link, focus-visible, alt en imágenes, contraste AA.

## Enlaces cruzados

4º ESO es **bisagra hacia Bachillerato**. En el hub de cada unidad hay dos secciones:

- **🔁 Repaso de cursos anteriores** → TyD 2º/3º ESO
- **🔗 Conexión Bachillerato** → TECI II

| Unidad | Repaso | Profundización TECI II |
|---|---|---|
| U1 Vivienda | TyD2 U5 Electricidad (CGMP) | Bloque G — Tecnología Sostenible |
| U2 Energías renovables | — | Bloque G — Tecnología Sostenible |
| U3 Fabricación y diseño | TyD3 U2 Construcción de objetos | Bloque B |
| U5 Electrónica | TyD3 U5 Circuitos y robótica | Bloques D1 y D2 — Electrónica Digital |
| U6 Neumática e hidráulica | — | Bloques C31 y C32 — Neumática e Hidráulica |
| U7 Robótica | TyD3 U5 Circuitos y robótica | Bloque F — Sistemas Automáticos |

Modelo de referencia: `teci2-ies-jdq` (TECI II) y `tyd3-ies-jdq` (TyD 3º ESO).
