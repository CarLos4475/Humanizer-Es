<div align="center">

# Humanizer en Español

### Que tu texto se lea como tú.

Una skill para revisar textos en español: menos relleno, mejor ritmo y una voz adecuada para cada ocasión.

**60 patrones de edición · Español primero · Escolar, profesional y técnico · Licencia MIT**

[Instalar](#instalación) · [Antes y después](#antes-y-después) · [Cómo usarla](#cómo-usarla) · [Qué incluye](#qué-incluye)

</div>

---

¿Tu texto está lleno de «cabe destacar», «no es X, es Y» y párrafos que terminan diciendo lo mismo? **Humanizer en Español** le da a tu agente criterios concretos para revisar esas fórmulas, ordenar las ideas y conservar lo que quieres decir.

Trabaja con frases, estructura, puntuación y formato. También cuida algo fácil de perder al reescribir: tus datos, tu postura, tus matices y tu manera de hablar.

## Lo que aporta

| Qué aporta | En la práctica |
|---|---|
| **Español desde el principio** | Atiende a usos, ritmo y variedades del español. Conserva tú, usted o vos según el texto. |
| **60 patrones con criterio** | Cada ficha explica qué revisar, cómo intervenir y cuándo conviene conservar la construcción. |
| **Una voz para cada contexto** | Una tarea escolar, un correo formal, un mensaje y una app reciben tratamientos distintos. |
| **Fidelidad al contenido** | Protege cifras, citas, condiciones, términos técnicos y diferencias como «sugiere» frente a «demuestra». |
| **Edición proporcional** | Puede limpiar unas frases, reorganizar un párrafo o dejar intacto un texto que ya funciona. |
| **Un paquete ligero** | Un núcleo de unas 650 palabras y cinco referencias temáticas. Son instrucciones Markdown, sin servidor ni API propia. |

## Antes y después

Ejemplos ilustrativos de las decisiones que enseña la skill. La redacción exacta depende del agente, del texto y del encargo.

### 1. Una tarea escolar más clara

**Antes**

> Cabe destacar que la lectura desempeña un papel fundamental en el desarrollo del pensamiento crítico, permitiendo que los estudiantes analicen distintas ideas y formen sus propias opiniones.

**Después**

> Leer ayuda a los estudiantes a desarrollar el pensamiento crítico: les permite analizar distintas ideas y formar opiniones propias.

La idea sigue completa y llega antes al lector.

### 2. Un contraste que se puede decir directamente

**Antes**

> Esta herramienta no solo permite crear listas de tareas, sino que también ofrece la posibilidad de asignar responsables.

**Después**

> La herramienta permite crear listas de tareas y asignar responsables.

Las dos funciones quedan claras sin presentar su suma como una revelación.

### 3. El punto y coma usado para apilar ideas

**Antes**

> El alumnado prepara los borradores; el profesor revisa las entregas; las familias reciben el informe; la dirección consulta los resultados.

**Después**

> El alumnado prepara los borradores y el profesor revisa las entregas. Las familias reciben el informe y la dirección consulta los resultados.

Se conserva el reparto de funciones y se aligera la lectura. Una enumeración compleja o una cita pueden seguir necesitando punto y coma.

### 4. Un correo formal sin tanta ceremonia

**Antes**

> Por medio de la presente, me permito dirigirme a usted con el objetivo de solicitar una ampliación del plazo de entrega.

**Después**

> Le escribo para solicitar una ampliación del plazo de entrega.

El trato sigue siendo respetuoso.

### 5. Copy de producto que explica qué puedes hacer

**Antes**

> Una solución integral e innovadora diseñada para transformar la forma en que tu equipo trabaja. Permite crear tareas, asignarlas y consultar su estado.

**Después**

> Crea tareas, asígnalas y consulta su estado.

La revisión aprovecha las funciones conocidas. No añade promesas de velocidad, ahorro o seguridad.

### 6. Saber qué conservar

**Original**

> La entrega no es el martes, sino el jueves. La profesora corrigió la fecha esta mañana.

**Revisión**

> La entrega no es el martes, sino el jueves. La profesora corrigió la fecha esta mañana.

Aquí la negación corrige un dato necesario. Se conserva, igual que las cifras, las citas y los matices que aportan precisión.

## Instalación

Necesitas un agente que admita [Agent Skills](https://agentskills.io/home), como Codex o Claude Code. La skill aporta las instrucciones; el agente realiza la revisión.

### Con el instalador de skills

Si tienes Node.js 22.20 o posterior, ejecuta:

```bash
npx skills add CarLos4475/Humanizer-Espa-ol --skill humanizer-es
```

El [instalador de skills](https://github.com/vercel-labs/skills) te permite elegir el agente. Por defecto la instala en el proyecto actual. Para usarla en todos tus proyectos, añade `-g`:

```bash
npx skills add CarLos4475/Humanizer-Espa-ol --skill humanizer-es -g
```

### Instalación manual

1. [Descarga el repositorio](https://github.com/CarLos4475/Humanizer-Espa-ol/archive/refs/heads/main.zip) y descomprímelo.
2. Copia la carpeta **`skills/humanizer-es` completa**, incluido `references`, a la ubicación que corresponda:

| Agente | Para todos tus proyectos | Solo en un proyecto |
|---|---|---|
| Codex | `~/.agents/skills/humanizer-es/` | `.agents/skills/humanizer-es/` |
| Claude Code | `~/.claude/skills/humanizer-es/` | `.claude/skills/humanizer-es/` |

`~` representa tu carpeta de usuario. La ruta del proyecto se toma desde su carpeta principal. Puedes consultar la documentación de [Codex](https://learn.chatgpt.com/docs/build-skills) y [Claude Code](https://code.claude.com/docs/en/skills) para ver cómo carga skills cada herramienta.

## Cómo usarla

Una vez instalada, pídeselo a tu agente con naturalidad:

```text
Humaniza este texto para una tarea de bachillerato.
Conserva mis ideas y las citas. Devuelve solo la versión final.

[Tu texto]
```

Para indicarla expresamente, usa `$humanizer-es` en Codex o `/humanizer-es` en Claude Code.

Puedes afinar el encargo:

| Si quieres… | Puedes pedir… |
|---|---|
| Una limpieza ligera | «Haz cambios mínimos. Quita el relleno y conserva mi estructura». |
| Mantener tu voz | «Toma este párrafo como muestra de cómo escribo». |
| Revisar un trabajo escolar | «Conserva la tesis, los ejemplos y el nivel de la tarea». |
| Un correo formal | «Mantén el trato de usted y haz la petición más directa». |
| Mejorar una explicación técnica | «Conserva términos, cifras, condiciones y pasos». |
| Escribir para una app o web | «Usa solo las funciones y el comportamiento que te describo». |

El agente puede elegirla automáticamente cuando el encargo coincide con su descripción. Mencionarla expresamente ayuda cuando quieres asegurarte de que la use.

## Qué incluye

```text
Humanizer-Espa-ol/
├── README.md
├── LICENSE
├── CONTRIBUTING.md
├── docs/
│   └── METODOLOGIA.md
└── skills/
    └── humanizer-es/
        ├── SKILL.md
        └── references/
            ├── patrones.md
            ├── registros.md
            ├── fidelidad-y-gramatica.md
            ├── fuentes.md
            └── evaluacion.md
```

El [núcleo de la skill](skills/humanizer-es/SKILL.md) reúne las decisiones esenciales. Las referencias desarrollan el [catálogo de patrones](skills/humanizer-es/references/patrones.md), los [registros y ejemplos](skills/humanizer-es/references/registros.md), la [fidelidad y gramática](skills/humanizer-es/references/fidelidad-y-gramatica.md), las [fuentes](skills/humanizer-es/references/fuentes.md) y las [pruebas de mantenimiento](skills/humanizer-es/references/evaluacion.md).

## Investigación y pruebas

La guía se apoya en estudios sobre escritura de modelos de lenguaje, corpus en español y recomendaciones de escritura clara. Distingue los hallazgos empíricos de las decisiones editoriales del proyecto.

La versión de partida se revisó con **60 salidas en cinco contextos nuevos**, usando doce encargos por contexto. Se comprobaron, entre otras cosas, datos, citas, condiciones técnicas, comparaciones, destinatarios y usos válidos de puntuación. Es una evaluación exploratoria con textos breves; el comportamiento puede variar entre agentes y tareas.

Los patrones sirven para editar con criterio. Una frase aislada no identifica al autor de un texto y la skill no promete resultados en detectores de IA. Puedes leer el alcance y los límites en la [metodología](docs/METODOLOGIA.md).

## Súmate

¿Encontraste una frase que sigue sonando acartonada, un cambio que pierde significado o un uso regional que debería conservarse? [Abre un issue](https://github.com/CarLos4475/Humanizer-Espa-ol/issues) con un ejemplo breve. La [guía de contribución](CONTRIBUTING.md) explica qué información resulta útil.

## Licencia

[MIT](LICENSE). Puedes usar, adaptar y compartir la skill conservando el aviso de licencia.
