# CLAUDE.md — awesome-ceuta-y-melilla

## Propósito

Selección de software open source que da **soporte específico a las ciudades autónomas de Ceuta y Melilla** — sus gobiernos locales, puertos, instituciones sanitarias, centros educativos e infraestructuras. Todo el contenido en español. El foco son Ceuta y Melilla: el software debe dirigirse específicamente a estas ciudades autónomas o a sus instituciones.

## Ámbito

- **Dos ciudades autónomas** situadas en el norte de África, en la costa mediterránea del continente africano.
- **Ceuta** (población ~84.000): ciudad autónoma fronteriza con Marruecos, con un importante puerto comercial y pesquero.
- **Melilla** (población ~87.000): ciudad autónoma fronteriza con Marruecos, con puerto y patrimonio arquitectónico modernista.
- No tienen universidades propias — solo **campus de la UNED** (Universidad Nacional de Educación a Distancia) y extensiones de la Universidad de Granada.
- **Instituciones**: Ciudad Autónoma de Ceuta, Ciudad Autónoma de Melilla, Puertos del Estado (autoridades portuarias de Ceuta y Melilla), INGESA (Instituto Nacional de Gestión Sanitaria — gestiona la sanidad en Ceuta y Melilla al no tener competencias transferidas), Delegaciones del Gobierno.

## Criterios de inclusión

### Incluir

- Software que interactúa con la **Ciudad Autónoma de Ceuta** o sus organismos (Sede Electrónica, datos abiertos).
- Software que interactúa con la **Ciudad Autónoma de Melilla** o sus organismos.
- Herramientas para **INGESA** en Ceuta y Melilla (gestión sanitaria).
- Software relacionado con los **puertos de Ceuta y Melilla** (autoridades portuarias, tráfico marítimo, ferry).
- Herramientas de **datos abiertos** de Ceuta y Melilla.
- Software sobre **transporte** en Ceuta y Melilla (autobuses, ferry al continente, paso fronterizo).
- Herramientas de **cartografía y SIG** específicas de Ceuta y Melilla.
- Software sobre la **frontera** con Marruecos (paso fronterizo del Tarajal en Ceuta, paso fronterizo de Beni Enzar en Melilla).
- Proyectos de la **UNED** cuando sean específicos de Ceuta o Melilla.
- Software de **turismo y patrimonio** de Ceuta y Melilla (fortificaciones, Melilla la Vieja, murallas reales de Ceuta).
- Proyectos de **medio ambiente** específicos (parque marítimo, reservas naturales).
- Software sobre **deportes** de Ceuta y Melilla (AD Ceuta, UD Melilla).
- Proyectos del **sistema sanitario** gestionado por INGESA.
- Software **educativo** específico (centros educativos, extensiones universitarias).

### No incluir

- Software **genérico** que funciona en toda España sin funcionalidad específica de Ceuta o Melilla — eso pertenece a awesome-spain.
- Software de **ámbito europeo** — eso pertenece a awesome-europe.
- Software de **otras comunidades autónomas** españolas.
- Software creado por ceutíes o melillenses que **no tiene funcionalidad específica** de estas ciudades.
- Repositorios **archivados o de solo lectura** — van a `DELETED.md`.
- Repos donde el autor indica que el proyecto está **roto, sin mantenimiento o deprecado**.
- Repos **sin README significativo** o que son claramente repos de test/experimento.
- Ejercicios de clase o trabajos académicos sin utilidad real.

### Zona gris — usar criterio

- Proyectos de la UNED que podrían ser genéricos — incluir si tienen datos o configuración específica de Ceuta o Melilla.
- Software que cubre Ceuta o Melilla junto con otras regiones — incluir si Ceuta o Melilla es un foco principal.

## Estándares de calidad

**Mismo listón que [awesome-spain](https://github.com/GeiserX/awesome-spain):**

- **No repos archivados**: si se descubre archivado tras la inclusión, mover a `DELETED.md` inmediatamente.
- **No repos extremadamente sin mantenimiento**: al menos un commit en los últimos 3 años, salvo que sea un proyecto claramente estable/completo.
- **No repos rotos**: si el README dice «deprecated», «no longer maintained», «use X instead» o similar — no incluir. Mover a `DELETED.md` si ya está listado.
- **Estrellas mínimas**: preferir repos con al menos unas pocas estrellas, pero herramientas nicho excepcionales con 0-1 estrellas pueden incluirse si cubren un hueco importante.
- **Verificar cada repo** antes de añadir: comprobar `archived`, `pushed_at`, `stargazers_count` vía `gh api repos/owner/name`.

## Formato de entrada

```markdown
- [Nombre](https://github.com/owner/repo) [![Stars](...)](stargazers) [![Last Commit](...)](commits) [![Language](...)](repo) [![License](...)](LICENSE) [![Tag](...)](url) - Descripción que empieza en mayúscula y termina con punto.
```

Las insignias se generan automáticamente con `scripts/transform-readme.py`. Para contribuir, basta con añadir la entrada en formato simple:

```markdown
- [Nombre](https://github.com/owner/repo) - Descripción que empieza en mayúscula y termina con punto.
```

- La descripción **no debe empezar con el nombre** del proyecto.
- Máximo una línea por entrada.
- Validar con awesome-lint-extra: `python3 lint.py` o mediante el workflow de CI.
- Entradas en **orden alfabético** dentro de cada categoría.
- Categorías en **orden alfabético** en el índice y en el cuerpo del documento.
- Entradas en `DELETED.md` también en **orden alfabético** dentro de cada sección.
- Dentro de cada categoría, las entradas se organizan en subsecciones `### Ceuta` y `### Melilla`.

## Verificación antes de añadir

Antes de incluir un repositorio, comprobar:

- **Existe y es público**: el enlace de GitHub funciona y el repo no es privado.
- **No está archivado o de solo lectura**: si archivado, va a `DELETED.md` (sección «Archivados»).
- **No está deprecado**: comprobar si el README dice «deprecated», «unmaintained», «broken», «use X instead».
- **Actividad razonable**: al menos un commit en los últimos 3 años, salvo que sea un proyecto estable/completo.
- **No es un duplicado**: cruzar con `README.md` y `DELETED.md`.
- **Calidad mínima**: tiene documentación (README) y no es un repositorio vacío o de test.

## Pull requests y contribuciones

- Las PRs deben usar la plantilla en `.github/PULL_REQUEST_TEMPLATE.md`.
- **Obligatorio**: incluir en la PR la **URL del servicio, API o institución de Ceuta o Melilla** a la que el software da soporte.
- Plantillas de issues disponibles para sugerir proyectos (`anadir-proyecto.md`) y solicitar retirada (`retirar-proyecto.md`).

## Estructura

- Secciones con `##`, subsecciones con `### Ceuta` y `### Melilla`.
- Índice de contenido al principio entre comentarios `<!--lint disable/enable awesome-list-item-->`.
- Al final: sección Contribuir, Nota y Descargo de responsabilidad (como párrafos en negrita, no encabezados ##).

## Temas prohibidos

No se aceptan proyectos relacionados con: pornografía, contenido NSFW, loterías o apuestas, religión, política partidista.

## Difusión

- Notificar a los propietarios de repos abriendo un issue titulado «Listado en awesome-ceuta-y-melilla» con un breve mensaje en español (tuteo) ofreciendo retirar si lo prefieren. Solo 1 issue por organización/usuario — no spamear repos del mismo propietario.
- Publicar en comunidades de Ceuta y Melilla (foros locales, grupos de Telegram) tras alcanzar masa crítica.
- Enviar PR a [sindresorhus/awesome](https://github.com/sindresorhus/awesome) tras 30 días desde la creación del repo.

## Aprendizajes

- Ceuta y Melilla son comunidades muy pequeñas (~84k y ~87k habitantes) con presencia mínima en GitHub.
- No tienen universidades propias — solo campuses de la UNED y extensiones de la Universidad de Granada, lo que reduce la producción de software académico.
- La sanidad está gestionada por INGESA (ámbito estatal), no por un servicio autonómico propio.
- Los puertos son infraestructuras clave (conexión ferry con la Península y tráfico comercial con África).
- La frontera con Marruecos es un tema de gran relevancia local (paso del Tarajal en Ceuta, Beni Enzar en Melilla).
- Las búsquedas en GitHub por «ceuta» devuelven muchos resultados sobre aves playeras en Bahía de Ceuta (México) — filtrar siempre.
- Las búsquedas por «melilla» devuelven perfiles de usuario y estaciones meteorológicas de Uruguay — filtrar siempre.
- No se encontraron organizaciones gubernamentales oficiales de Ceuta ni Melilla en GitHub.
- SIG-SGCP tiene repos «Ceuta» y «Melilla» (GIS/cartografía) pero sin licencia ni descripción.
- La mayoría de repos encontrados son ejercicios de clase, proyectos de hackathon sin mantenimiento o repos sin licencia.

*Generated by [LynxPrompt](https://lynxprompt.com) CLI*

<!-- BEGIN BEADS INTEGRATION v:1 profile:minimal hash:6cd5cc61 -->
## Beads Issue Tracker

This project uses **bd (beads)** for issue tracking. Run `bd prime` to see full workflow context and commands.

### Quick Reference

```bash
bd ready              # Find available work
bd show <id>          # View issue details
bd update <id> --claim  # Claim work
bd close <id>         # Complete work
```

### Rules

- Use `bd` for ALL task tracking — do NOT use TodoWrite, TaskCreate, or markdown TODO lists
- Run `bd prime` for detailed command reference and session close protocol
- Use `bd remember` for persistent knowledge — do NOT use MEMORY.md files

**Architecture in one line:** issues live in a local Dolt DB; sync uses `refs/dolt/data` on your git remote; `.beads/issues.jsonl` is a passive export. See https://github.com/gastownhall/beads/blob/main/docs/SYNC_CONCEPTS.md for details and anti-patterns.

## Agent Context Profiles

The managed Beads block is task-tracking guidance, not permission to override repository, user, or orchestrator instructions.

- **Conservative (default)**: Use `bd` for task tracking. Do not run git commits, git pushes, or Dolt remote sync unless explicitly asked. At handoff, report changed files, validation, and suggested next commands.
- **Minimal**: Keep tool instruction files as pointers to `bd prime`; use the same conservative git policy unless active instructions say otherwise.
- **Team-maintainer**: Only when the repository explicitly opts in, agents may close beads, run quality gates, commit, and push as part of session close. A current "do not commit" or "do not push" instruction still wins.

## Session Completion

This protocol applies when ending a Beads implementation workflow. It is subordinate to explicit user, repository, and orchestrator instructions.

1. **File issues for remaining work** - Create beads for anything that needs follow-up
2. **Run quality gates** (if code changed) - Tests, linters, builds
3. **Update issue status** - Close finished work, update in-progress items
4. **Handle git/sync by active profile**:
   ```bash
   # Conservative/minimal/default: report status and proposed commands; wait for approval.
   git status

   # Team-maintainer opt-in only, unless current instructions forbid it:
   git pull --rebase
   git push
   git status
   ```
5. **Hand off** - Summarize changes, validation, issue status, and any blocked sync/commit/push step

**Critical rules:**
- Explicit user or orchestrator instructions override this Beads block.
- Do not commit or push without clear authority from the active profile or the current user request.
- If a required sync or push is blocked, stop and report the exact command and error.
<!-- END BEADS INTEGRATION -->

## Where the tracker syncs

This repo is public, so its tracker syncs only to the private Dolt remote named by `sync.remote` in `.beads/config.yaml` (`giteaer/awesome-ceuta-y-melilla-beads` on Gitea). The block above says sync uses "your git remote". Here that never means this GitHub repo. Don't add it as a Dolt remote and don't push `refs/dolt/*` to it.
