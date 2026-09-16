# Pendientes · Tecnología 4º ESO

Lista de lo que queda por completar.

## Material disperso de U5 y U6 (§7.1 del brief)

Manuel ha indicado que tiene "cosas pero poco" para U5 (Electrónica) y U6
(Neumática-hidráulica). En la fase de andamiaje, ambas unidades se han
tratado como cualquier otra sin material confirmado (badge "Próximamente"
en el index).

> **Pendiente integrar fragmentos del ecosistema TECI II adaptados al nivel 4º ESO:**
>
> - **U5 (Electrónica analógica y digital):** considerar fragmentos del
>   **Bloque D2 (Electrónica Digital)** de TECI II — álgebra de Boole,
>   simplificación de funciones, mapas de Karnaugh básicos, puertas lógicas.
>   Podría reutilizarse parcialmente la teoría introductoria adaptando el
>   lenguaje a 4º ESO.
> - **U6 (Neumática e hidráulica):** considerar fragmentos del **Bloque C3
>   (Neumática e Hidráulica)** de TECI II — esquemas con simbología ISO 1219,
>   cálculos de fuerza con Pascal, primeros circuitos con cilindros y válvulas.
>
> Manuel decidirá qué fragmentos reutilizar y en qué profundidad. Esto NO
> entra en el bootstrap actual; cuando llegue la fase específica
> (Fase I del brief, aplazada), se abrirá un sprint propio para esto.

## Pendientes de Manuel (no bloqueantes)

- [ ] **Criterios de evaluación LOMLOE concretos** por unidad. Rellenar el
  `<details class="criterios">` de cada hub.
- [ ] **Bullets de "saber/hacer/evaluar"**: los actuales son una primera
  aproximación al currículo LOMLOE Andalucía. Revisar y ajustar.
- [ ] **Duración estimada de las unidades**: rangos orientativos. Validar.
- [ ] **Proyectos integradores**: definir los proyectos del curso (típicamente
  un proyecto por evaluación: vivienda eficiente, robot autónomo, etc.).
- [ ] **Herramientas**: añadir simuladores (electrónica con Falstad, neumática
  con FluidSIM, robótica con Tinkercad Circuits), glosario.

## Auditoría de septiembre de 2026

Hecho: U6 (símbolos ISO 1219, circuitos dibujados, visor animado, quiz), U5 (simulador Karnaugh
con motor real, disposición de clase en libro y actividades, erratas), tests reequilibrados en
longitud (126 preguntas), 30 mA en U1, desbordes en móvil, enlaces «Repaso» a TyD2/TyD3,
sesiones coherentes hub/PROGRAMACION, README y KIT al día.

- [x] Figuras en los libros: comprobado el 16-sep-2026 que estaban **todas hechas** ya en la
  auditoría de septiembre — CGMP y agua (U1), lazo abierto/cerrado y patillaje UNO (U7),
  aditivo/sustractivo/conformado (U3 y U4), puertas en las dos normas, transistor y patillaje del
  7408 (U5). Lo que faltaba de verdad era U2, que no tenía ninguna; ya tiene tres.
- [x] Contenido con fecha revisado el 16-sep-2026 contra fuentes actuales: el reglamento europeo en
  vigor sigue fijando 0 g CO2/km en 2035 y la rebaja al 90 % que propuso la Comisión en diciembre de
  2025 está pendiente de Parlamento y Consejo (se explica así, no se da por hecho); A+++ sustituido
  por clase A o B (reescalado de 2021); ITER pasa a 2034 investigación y 2039 deuterio-tritio; y el
  cierre nuclear español ya no es 2027-2035, porque la prórroga de Almaraz (agosto de 2026) lo llevó
  a 2030.
- [ ] Ejemplos Arduino del libro de U7: `adelante()` y `giraDerecha()` no están definidas y
  falta `setup()`; indicar que son fragmentos o completarlos.
- [ ] En el simulador C31 de TECI II los orificios de la 3/2 están sobre el cuadrado del lado
  del pulsador; en la norma van sobre el de reposo (lado del muelle), como en 4º.
- [ ] Interactivos que siguen siendo test de texto sin dibujo: `identifica-material`,
  `proceso-fabricacion` y `elige-tecnologia` (los dos primeros sí tienen algo que dibujar).
- [ ] Calculadoras que ganarían con deslizador: `factura-luz`, `calculadora-solar`, `mix-energetico`,
  `binario`, `slicer-sim` y `lazo-control`. El patrón está en `cilindro-fuerza` y en el
  `relacion-transmision` de tyd3.
- [ ] Los 6 interactivos de dibujo técnico están duplicados byte a byte con tyd3.

## Infraestructura

- [x] Repo en git y worker desplegado (`tec4-ies-jdq.malonso72.workers.dev`), auto-deploy con `git push`.
- [ ] **Google Search Console**: añadir verificación si se quiere indexar.

## Enlaces cruzados (§7.3 del brief)

Los siguientes hubs llevan callout(s) de cross-link:

| Unidad | Repaso TyD3 | Profundización TECI II |
|---|---|---|
| U2 | — | `teci2.../teoria/bloque_G.html` (Sostenible) |
| U3 | `tyd3.../unidades/02-construccion-objetos/` | — |
| U5 | `tyd3.../unidades/05-circuitos-robotica/` | `teci2.../teoria/bloque_D2.html` (Digital) |
| U6 | — | `teci2.../teoria/bloque_C31.html` (Neumática) |
| U7 | `tyd3.../unidades/05-circuitos-robotica/` | `teci2.../teoria/bloque_F.html` (Automáticos) |

> Las URLs son absolutas a los subdominios Cloudflare hermanos. Cuando
> TyD3 y TECI II estén desplegados, los enlaces serán navegables. En local
> (`python -m http.server`) apuntan a un dominio externo (intencionalmente).
> U5 y U7 llevan los dos callouts: 4º ESO es bisagra entre 3º ESO y 2º Bach.

## Material confirmado

Ninguno en el bootstrap. Cuando llegue la Fase I (aplazada en el brief
v1.2.0 hasta que Manuel concrete), se abrirá un sprint específico.
