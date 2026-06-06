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

## Infraestructura

- [ ] **`git init`**: el sistema en el que se generó este repo no tenía
  git instalado. Manuel debe ejecutar al recibirlo:
  ```bash
  cd tec4-ies-jdq && git init -b main && git add . && \
  git commit -m "Bootstrap del sitio Tecnología 4º ESO [v1.0.0]"
  ```
- [ ] **Configuración del worker Cloudflare**: crear el subdominio
  `tec4-ies-jdq.malonso72.workers.dev`. Probar primer deploy con
  `npx wrangler deploy`.
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
