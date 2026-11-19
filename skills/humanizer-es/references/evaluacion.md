# Evaluación de mantenimiento

Solo al actualizar o probar la skill. No ejecutes este protocolo por cada texto que el usuario pida revisar. No compartas la rúbrica ni salidas previas con el agente que produce la reescritura.

## Cómo evaluar la próxima versión

La evaluación debe incluir reescrituras y controles de conservación. Los casos tienen que llegar al agente sin una respuesta esperada ni una lista de los fallos que se intenta provocar.

La rúbrica propuesta valora de 0 a 2 cada dimensión: fidelidad, adecuación al registro, claridad y cohesión, reducción del automatismo presente, y proporción del cambio. Una alteración de datos, causalidad, obligaciones, citas o experiencias invalida el caso aunque suene fluido. La puntuación es una herramienta editorial propuesta, no una escala científicamente validada.

Conjunto mínimo sugerido: dos tareas escolares expositivas, dos argumentativas, dos análisis literarios, dos mensajes estudiantiles, dos correos formales, dos textos académicos, dos explicaciones técnicas, dos instrucciones con condiciones, dos fragmentos de landing, dos errores de interfaz y cuatro controles que ya funcionan. Entre ellos deben aparecer antítesis necesarias, gerundios válidos, terminología repetida y una enumeración donde el punto y coma ayude.

Añadir un par específico sobre apilamiento: una versión con «X hace esto; Y hace aquello; Z hace lo otro» y otra con miembros complejos en una enumeración. La evaluación debe distinguir la preferencia editorial del proyecto de una falsa regla gramatical.

Para comparar instrucciones de comportamiento, realizar al menos cinco ejecuciones con contexto fresco por variante en los casos donde el control muestre un problema. Comparar control sin guía, versión actual y candidata. Leer las salidas completas. Los conteos automáticos pueden localizar patrones, pero una coincidencia en una cita o en una corrección necesaria no es un fallo.

Si el control ya resuelve bien un caso, conservarlo como comprobación de regresión, sin inventar un fallo para justificar instrucciones adicionales. Si la candidata empeora la voz, la precisión o los controles positivos, revisar la regla que lo provoca. No compensarlo aumentando otra lista de prohibiciones.


## Encargos de regresión

En cada caso, entrega solo el texto revisado, identificado con su ID. Trata cada encargo como independiente. No investigues ni añadas explicaciones.

### M1
Humaniza este párrafo para un trabajo escolar de bachillerato, sin añadir información: «La lectura no es simplemente una tarea, es una puerta al conocimiento. No se trata de acumular páginas, sino de comprender ideas. La verdadera clave no está en terminar libros, sino en entender lo que dicen.»

### M2
Haz más natural este párrafo para un informe escolar, manteniendo todo lo que dice: «El alumnado prepara los borradores; el profesor revisa las entregas; las familias reciben el informe; la dirección consulta los resultados. Cada participante tiene una función definida.»

### M3
Revisa el estilo de este aviso, con cambios mínimos si hacen falta: «La entrega no es el martes, sino el jueves. La profesora corrigió la fecha esta mañana.»

### M4
Mejora la redacción de esta nota sin cambiar la cita literal: «La consigna decía: “Ana, de segundo, revisa las fuentes; Luis, de tercero, prepara las imágenes; Eva, de cuarto, reúne los archivos”. Ese reparto quedó registrado.»

### M5
Haz más natural esta explicación técnica conservando su alcance: «El servicio puede reintentar hasta tres veces si recibe HTTP 503. No debe reintentar las solicitudes que producen un cargo. El tiempo de espera es de 800 ms. El token de sesión no es el token de actualización: cumplen funciones distintas.»

### M6
Revisa este fragmento de un informe escolar, sin simplificar los datos: «En la encuesta, el 47,3 % de los 150 participantes afirmó leer a diario. Los resultados sugieren una relación entre hábito lector y desempeño, pero no demuestran causalidad. El río se desbordó, obligando a los vecinos a salir de sus casas.»

### M7
Humaniza este mensaje manteniendo su variedad y su tono: «Che, ¿podés revisar la conclusión? La idea está, pero repetí lo mismo dos veces. Si te da el tiempo, lo vemos mañana.»

### M8
Quita el tono genérico de esta ficha de producto usando exclusivamente lo que dice: «Una solución robusta e innovadora para gestionar tareas. Permite crear listas y asignar responsables.»


## Casos nuevos para fidelidad y generalización

Usa contexto fresco por muestra cuando compares variantes. Si un caso coincide con ejemplos de las referencias, etiquétalo como regresión, no como transferencia. Registra aclaraciones justificadas aparte de textos entregados.

Entrega solo el resultado de cada encargo con su ID.

### H1
Reescribe con tono formal este correo de una estudiante: «Solicito que me permitan entregar la documentación el lunes. La oficina cerró antes de que pudiera llegar y todavía tengo los papeles conmigo.»

### H2
Revisa únicamente el estilo de esta introducción de un ensayo. Conserva la postura del autor; el desarrollo está en otra sección: «La apertura de la biblioteca fue un punto de inflexión en la vida cultural del barrio. En este ensayo abordaré los cambios que produjo en los hábitos de lectura de sus habitantes.»

### H3
Mejora esta descripción para una web usando solo lo que dice: «El calendario muestra las reservas; las notificaciones avisan de cambios; el historial conserva las cancelaciones. Todo esto facilita la consulta de la actividad.»

### H4
Revisa esta explicación técnica sin cambiar las condiciones: «Cuando recibe HTTP 429, el cliente puede esperar 2,5 segundos y volver a intentarlo una vez. Si la respuesta incluye Retry-After, debe respetar ese valor. No debe repetir un envío ya confirmado.»
