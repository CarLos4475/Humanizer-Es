# Cómo se construyó la guía

Humanizer en Español reúne criterios de edición para mejorar prosa española y conservar lo que su autor quiere decir. La investigación de apoyo distingue cuatro bases:

| Marca | Base de la recomendación |
|---|---|
| ES | Evidencia empírica que incluye español, limitada a los modelos y géneros estudiados |
| OT | Evidencia en otras lenguas cuya aplicación al español necesita criterio y pruebas |
| ED | Recomendación editorial o gramatical |
| PR | Preferencia editorial adoptada por este proyecto |

Las marcas aparecen en el catálogo. No asignan una probabilidad de autoría ni hacen incorrecta una construcción por su sola presencia.

## Fuentes

Se consultaron investigaciones originales sobre variación de estilo, vocabulario, antítesis y textos humanos frente a textos de modelos. Para español, el proyecto ROBOT-TALK y estudios vinculados ofrecen comparaciones por género. La guía utiliza también documentación de RAE y ASALE, escritura clara, documentación técnica y contenido de interfaces.

Los resultados en inglés o mandarín no se presentan como mediciones del español. Tampoco se descargó ni se replicó un corpus completo para producir frecuencias propias. Las fuentes, sus alcances y sus límites se recogen en [fuentes.md](../skills/humanizer-es/references/fuentes.md).

## Qué se probó

Durante la revisión se compararon un control sin guía, la versión anterior y candidatas sucesivas. Se usaron encargos escolares, formales, casuales, académicos, técnicos y de producto. Las observaciones sirvieron para corregir pérdida de comparaciones, inferencias sobre destinatarios y cambios indebidos en la postura del autor.

La versión corregida recibió una última pasada de cinco contextos nuevos, con doce encargos por contexto: **60 salidas**. Se revisaron ocho casos de regresión y cuatro adicionales sobre destinatario desconocido, una tesis en un fragmento, puntuación apilada e instrucciones técnicas. Se leyeron las salidas y se comprobaron invariantes concretos, como citas, cifras y condiciones.

Los doce encargos de cada lote compartían contexto. Una ejecución nueva no equivale a un contexto independiente por texto. Algunos casos se solapan con ejemplos de las referencias y se consideran pruebas de regresión. La cobertura más amplia de registros se realizó en una candidata anterior; no se atribuyen todas sus salidas a la última versión.

## Cómo interpretar los resultados

La evaluación fue exploratoria y utilizó textos breves construidos para las pruebas. No hubo un corpus escolar representativo, una escala de calidad validada ni una estimación estadística de superioridad. Los resultados pueden cambiar con el modelo, el encargo y la longitud del documento.

El protocolo de mantenimiento propone valorar fidelidad, adecuación al registro, claridad, reducción del automatismo presente y proporción del cambio. La métrica principal no es eliminar palabras o signos: una revisión debe mantener el contenido y resolver el problema del pasaje.

## Dos decisiones de estilo

**Contrastes de plantilla.** La guía reduce «no es X, es Y» y construcciones afines cuando añaden énfasis vacío o niegan una alternativa irrelevante. Conserva correcciones, distinciones y comparaciones que sostienen el argumento.

**Punto y coma apilado.** El proyecto favorece reorganizar las cadenas mecánicas de afirmaciones. El signo sigue siendo válido en citas y enumeraciones complejas. Esta preferencia no se presenta como regla gramatical ni como señal universal de IA.

Para probar futuras modificaciones, consulta [evaluacion.md](../skills/humanizer-es/references/evaluacion.md). Para proponer un caso, sigue la [guía de contribución](../CONTRIBUTING.md).
