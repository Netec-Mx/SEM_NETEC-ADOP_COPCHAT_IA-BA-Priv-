# Ejercicio práctico: Redactar y refinar solicitudes a Copilot Chat aplicando contexto, objetivo y expectativas

## Metadata

| Campo | Detalle |
|-------|---------|
| **Duración** | 30 minutos |
| **Complejidad** | Media |
| **Nivel Bloom** | Aplicar |
| **Tecnologías** | Microsoft Copilot Chat (web), Microsoft Edge, OneDrive for Business, Microsoft Word |

## Descripción General

En este laboratorio aplicarás de forma práctica el marco COFE (Contexto, Objetivo, Fuentes, Expectativas) para transformar solicitudes vagas en prompts estructurados de alta calidad. Trabajarás con tres escenarios corporativos distintos usando el contexto de Contoso Corp: redacción de comunicación interna, análisis de resultados de satisfacción y generación de descripciones para imágenes. Para cada escenario compararás los resultados de un prompt básico contra un prompt estructurado, ejecutarás refinamientos iterativos y documentarás todo en un catálogo reutilizable de prompts.

## Objetivos de Aprendizaje

Al completar este laboratorio serás capaz de:

- [ ] Identificar y aplicar los cuatro componentes de un prompt de calidad (Contexto, Objetivo, Fuentes, Expectativas) en solicitudes reales a Copilot Chat
- [ ] Comparar cualitativamente los resultados obtenidos con prompts simples versus prompts estructurados con el marco COFE
- [ ] Personalizar solicitudes según el tipo de tarea: redacción, análisis y generación creativa
- [ ] Aplicar al menos dos rondas de refinamiento iterativo mediante solicitudes de seguimiento
- [ ] Documentar un catálogo personal de prompts efectivos reutilizables en formato Word

## Prerrequisitos

### Conocimientos Previos

| Requisito | Descripción |
|-----------|-------------|
| Lab 01-03-01 completado | Formulario "Formulario-Satisfaccion-Hibrido" creado en Microsoft Forms con datos ficticios |
| Lab 02-03-01 completado | Archivo "Banner-Hibrido-Final.png" generado con Microsoft Designer |
| Marco COFE | Comprensión teórica de los cuatro componentes de una solicitud efectiva (lección 3.1) |
| Navegación Copilot Chat | Experiencia básica accediendo a copilot.microsoft.com e interactuando con la interfaz |

### Acceso y Recursos Requeridos

| Recurso | Detalle |
|---------|---------|
| Cuenta corporativa | usuario@contoso-curso.onmicrosoft.com con licencia Copilot for Microsoft 365 activa |
| Carpeta Lab03 | `OneDrive\Curso-M365-Copilot\Lab03\` creada y sincronizada |
| Documento de contexto | `OneDrive\Curso-M365-Copilot\Recursos-Compartidos\Contexto-Contoso-Corp.pdf` disponible |
| Archivo Lab 01 | `OneDrive\Curso-M365-Copilot\Lab01\Formulario-Satisfaccion-Hibrido.docx` disponible |
| Archivo Lab 02 | `OneDrive\Curso-M365-Copilot\Lab02\Banner-Hibrido-Final.png` disponible |

## Entorno del Laboratorio

### Software Requerido

| Aplicación | Versión | Propósito |
|------------|---------|-----------|
| Microsoft Edge | 124.0.2478.105 | Navegador para acceder a Copilot Chat |
| Microsoft Copilot Chat | Versión web (copilot.microsoft.com) | Plataforma principal de interacción con IA |
| Microsoft Word | Versión 2405 (Build 17628.20144) | Documentación del catálogo de prompts |
| OneDrive for Business | Versión sync 24.071.0407.0003 | Almacenamiento y organización de archivos |

### Verificación Inicial del Entorno

1. Abre Microsoft Edge y navega a `https://copilot.microsoft.com`
2. Inicia sesión con tu cuenta corporativa del curso
3. **Verifica** que aparezca el mensaje: *"Tu organización tiene protección de datos comerciales activada"*
4. Confirma que la carpeta `OneDrive\Curso-M365-Copilot\Lab03\` existe navegando a `https://onedrive.live.com` o mediante el explorador de archivos sincronizado

> ⚠️ **IMPORTANTE**: Si NO aparece el mensaje de protección de datos comerciales, detente y notifica al instructor antes de continuar.

---

## Procedimiento Paso a Paso

### Paso 1: Crear el documento de catálogo de prompts

**Objetivo:** Preparar el documento donde registrarás todos los prompts, resultados y observaciones del laboratorio.

**Instrucciones:**

1. Abre Microsoft Word desde el menú de aplicaciones o el escritorio.
2. Crea un nuevo documento en blanco.
3. Escribe el siguiente encabezado en la primera línea:

```
Catálogo de Prompts Efectivos — Lab 03-01-01
Participante: [Tu nombre completo]
Fecha: [Fecha actual]
Empresa ficticia: Contoso Corp
```

4. Debajo del encabezado, crea la siguiente estructura de secciones usando el estilo **Título 1** para cada una:

```
Escenario 1: Comunicación Interna — Correo sobre Política Híbrida
Escenario 2: Análisis — Resumen de Resultados de Satisfacción
Escenario 3: Generación Creativa — Descripción de Imagen
Reflexiones y Aprendizajes
```

5. Dentro de cada sección de escenario, crea los siguientes subtítulos con estilo **Título 2**:

```
Prompt Básico (sin estructura)
Resultado del Prompt Básico
Prompt Estructurado (marco COFE)
Resultado del Prompt Estructurado
Comparación de Resultados
Refinamiento Iterativo — Ronda 1
Refinamiento Iterativo — Ronda 2
```

6. Guarda el archivo como `Catalogo-Prompts-Lab03.docx` en la ruta `OneDrive\Curso-M365-Copilot\Lab03\`.

**Resultado esperado:** Un documento Word con la estructura completa de secciones listo para ser completado durante el laboratorio.

**Verificación:** El archivo aparece en `OneDrive\Curso-M365-Copilot\Lab03\` y contiene las cuatro secciones principales con sus respectivos subtítulos.

---

### Paso 2: Escenario 1 — Prompt básico para comunicación interna

**Objetivo:** Enviar un prompt simple (sin estructura COFE) a Copilot Chat para redactar un correo sobre la política híbrida y registrar el resultado como línea base.

**Instrucciones:**

1. En Microsoft Edge, asegúrate de estar en `https://copilot.microsoft.com` con tu cuenta corporativa.
2. Inicia una **nueva conversación** haciendo clic en "Nuevo tema" o el ícono correspondiente.
3. Escribe el siguiente prompt básico exactamente como aparece:

```
Escribe un correo sobre la política de trabajo híbrido de la empresa.
```

4. Presiona **Enter** y espera la respuesta completa de Copilot.
5. Lee la respuesta generada y observa:
   - ¿El tono es apropiado para Contoso Corp?
   - ¿Menciona datos específicos (3 días presencial, 2 remoto)?
   - ¿Tiene un destinatario claro?
   - ¿El formato es adecuado para un correo interno corporativo?
6. Copia la respuesta completa de Copilot.
7. Regresa a tu documento `Catalogo-Prompts-Lab03.docx`.
8. Pega la respuesta bajo la sección **"Resultado del Prompt Básico"** del Escenario 1.
9. Registra el prompt utilizado bajo **"Prompt Básico (sin estructura)"**.

**Resultado esperado:** Copilot genera un correo genérico sobre trabajo híbrido, probablemente sin datos específicos de Contoso Corp, con tono indefinido y sin estructura clara de comunicación corporativa.

**Verificación:** El prompt y su resultado están documentados en las secciones correspondientes del documento Word.

---

### Paso 3: Escenario 1 — Prompt estructurado con marco COFE

**Objetivo:** Reescribir la solicitud aplicando los cuatro componentes del marco COFE y comparar la diferencia en calidad de respuesta.

**Instrucciones:**

1. En Copilot Chat, inicia una **nueva conversación** (es importante no continuar la anterior para evitar sesgo contextual).
2. Escribe el siguiente prompt estructurado:

```
[Contexto] Soy el gerente de Comunicaciones Internas de Contoso Corp, una empresa de tecnología con 500 empleados. La empresa acaba de implementar una política de trabajo híbrido: 3 días presenciales (lunes, martes y jueves) y 2 días remotos (miércoles y viernes). Los datos de nuestra encuesta interna muestran que el 72% de los empleados están satisfechos, el 18% son neutrales y el 10% están insatisfechos con esta política.

[Objetivo] Redacta un correo electrónico interno dirigido a todos los colaboradores que refuerce los beneficios de la política híbrida, reconozca las preocupaciones del 10% insatisfecho y anuncie una sesión abierta de preguntas y respuestas con el equipo de Recursos Humanos la próxima semana.

[Fuentes] Usa los datos de satisfacción proporcionados (72% satisfechos, 18% neutrales, 10% insatisfechos) y el esquema de días presenciales/remotos descrito arriba.

[Expectativas] El correo debe tener un tono profesional pero cercano, máximo 300 palabras, con un asunto atractivo, saludo inclusivo, tres párrafos (beneficios, reconocimiento de preocupaciones, invitación a sesión Q&A) y un cierre con firma del equipo de Comunicaciones Internas. Formato de correo electrónico corporativo.
```

3. Presiona **Enter** y espera la respuesta completa.
4. Lee la respuesta y evalúa:
   - ¿Incluye los datos específicos de Contoso Corp (72%, 18%, 10%)?
   - ¿Respeta la estructura de tres párrafos solicitada?
   - ¿El tono es profesional pero cercano?
   - ¿Incluye asunto, saludo y firma?
   - ¿Está dentro de las 300 palabras?
5. Copia el prompt y la respuesta al documento `Catalogo-Prompts-Lab03.docx` en las secciones correspondientes del Escenario 1.
6. En la sección **"Comparación de Resultados"**, escribe 3-5 oraciones describiendo las diferencias clave entre ambas respuestas.

**Resultado esperado:** Copilot genera un correo específico para Contoso Corp con datos reales, estructura de tres párrafos, tono apropiado, asunto incluido y extensión controlada. La diferencia con el prompt básico debe ser evidente.

**Verificación:** El prompt COFE y su resultado están documentados. La sección de comparación contiene al menos 3 diferencias observadas entre el resultado básico y el estructurado.

---

### Paso 4: Escenario 1 — Refinamiento iterativo

**Objetivo:** Aplicar dos rondas de refinamiento para mejorar progresivamente el correo generado, practicando la técnica de solicitudes de seguimiento.

**Instrucciones:**

1. **Sin iniciar nueva conversación** (continúa en la misma), escribe la primera solicitud de refinamiento:

```
Refinamiento 1: El correo está bien, pero necesito que hagas estos ajustes:
- Agrega una línea específica que mencione que los empleados insatisfechos pueden agendar una reunión confidencial con su líder directo antes de la sesión Q&A.
- Cambia el cierre para incluir un enlace ficticio a un formulario de retroalimentación anónima: https://forms.contoso.com/feedback-hibrido
- Haz el primer párrafo más conciso (máximo 2 oraciones).
```

2. Presiona **Enter** y revisa la respuesta actualizada.
3. Copia el prompt de refinamiento y la nueva respuesta bajo **"Refinamiento Iterativo — Ronda 1"** en tu documento.
4. Ahora escribe la segunda solicitud de refinamiento:

```
Refinamiento 2: Casi perfecto. Últimos ajustes:
- Agrega un emoji profesional (📅) antes de la fecha de la sesión Q&A para hacerlo más visual.
- Incluye un "P.D." al final que diga que la política será revisada trimestralmente con base en la retroalimentación recibida.
- Asegúrate de que el asunto del correo no supere 8 palabras.
```

5. Presiona **Enter** y revisa la versión final.
6. Copia el prompt y la respuesta bajo **"Refinamiento Iterativo — Ronda 2"**.

**Resultado esperado:** Cada ronda de refinamiento produce una versión mejorada del correo que incorpora los cambios solicitados sin perder los elementos positivos de la versión anterior. La versión final es un correo listo para enviar.

**Verificación:** Ambas rondas de refinamiento están documentadas con sus prompts y resultados. La versión final del correo incluye todos los elementos solicitados: enlace al formulario, opción de reunión confidencial, emoji, P.D. y asunto de máximo 8 palabras.

---

### Paso 5: Escenario 2 — Análisis de resultados de satisfacción

**Objetivo:** Aplicar el marco COFE para una tarea de análisis, usando como fuente los datos del formulario creado en el Lab 01-03-01.

**Instrucciones:**

1. Antes de ir a Copilot Chat, abre el archivo `OneDrive\Curso-M365-Copilot\Lab01\Formulario-Satisfaccion-Hibrido.docx` y revisa brevemente los datos de la encuesta (o consulta el documento `Contexto-Contoso-Corp.pdf` para los datos de satisfacción: 72% satisfechos, 18% neutrales, 10% insatisfechos).
2. En Copilot Chat, inicia una **nueva conversación**.
3. Primero, envía un **prompt básico** como línea base:

```
Resume los resultados de una encuesta de satisfacción sobre trabajo híbrido.
```

4. Registra el prompt y la respuesta en la sección correspondiente del Escenario 2 de tu documento.
5. Ahora inicia una **nueva conversación** y envía el prompt estructurado con marco COFE:

```
[Contexto] Soy analista de Recursos Humanos en Contoso Corp (500 empleados, sector tecnología). Acabamos de cerrar la encuesta trimestral de satisfacción sobre nuestra política de trabajo híbrido (3 días presenciales, 2 remotos). Participaron 387 de 500 empleados (tasa de respuesta: 77.4%).

[Objetivo] Analiza los resultados y genera un resumen ejecutivo que identifique patrones clave, áreas de preocupación y recomendaciones accionables para el Comité de Dirección.

[Fuentes] Datos de la encuesta:
- Satisfacción general: 72% satisfechos, 18% neutrales, 10% insatisfechos
- Principales motivos de insatisfacción (del 10%): dificultad para colaborar en días remotos (45%), sensación de desconexión con el equipo (35%), problemas técnicos de conectividad (20%)
- Principales beneficios percibidos (del 72%): mejor balance vida-trabajo (68%), ahorro en transporte (52%), mayor concentración en días remotos (47%)
- Departamentos con mayor insatisfacción: Ingeniería (15% insatisfechos) y Ventas (13% insatisfechos)

[Expectativas] Formato de resumen ejecutivo de una página con: título, resumen en una oración, sección de hallazgos clave (viñetas), sección de áreas de riesgo (viñetas), y tres recomendaciones concretas con responsable sugerido y plazo. Tono analítico y orientado a la acción. Máximo 400 palabras.
```

6. Registra el prompt y la respuesta en las secciones correspondientes.
7. Escribe la comparación entre ambos resultados (3-5 oraciones).
8. Aplica **una ronda de refinamiento**:

```
Refinamiento: Agrega al inicio una tabla resumen con los KPIs principales (tasa de respuesta, % satisfacción, % insatisfacción, departamentos críticos) y al final una nota que indique que este resumen se presentará en la reunión del Comité de Dirección del próximo lunes. Mantén el resto sin cambios.
```

9. Registra el refinamiento y su resultado.
10. Aplica una **segunda ronda de refinamiento**:

```
Refinamiento 2: En las recomendaciones, asegúrate de que al menos una esté vinculada directamente a resolver los problemas técnicos de conectividad del 20% que los reportó. Además, agrega entre paréntesis el nivel de prioridad de cada recomendación: (Alta), (Media) o (Baja).
```

11. Registra y guarda.

**Resultado esperado:** El prompt estructurado genera un resumen ejecutivo con estructura clara, datos específicos de Contoso Corp, recomendaciones accionables con responsables y plazos. Los refinamientos agregan la tabla de KPIs y priorizan las recomendaciones.

**Verificación:** El Escenario 2 tiene documentados: prompt básico + resultado, prompt COFE + resultado, comparación, y dos rondas de refinamiento con sus respectivos resultados.

---

### Paso 6: Escenario 3 — Generación creativa de descripción de imagen

**Objetivo:** Aplicar el marco COFE para una tarea de generación creativa, creando una descripción mejorada para una variante del banner generado en el Lab 02-03-01.

**Instrucciones:**

1. Abre el archivo `OneDrive\Curso-M365-Copilot\Lab02\Banner-Hibrido-Final.png` para recordar la imagen que generaste previamente.
2. En Copilot Chat, inicia una **nueva conversación**.
3. Envía el **prompt básico**:

```
Dame una descripción para generar una imagen sobre trabajo híbrido.
```

4. Registra el prompt y resultado en el Escenario 3 de tu documento.
5. Inicia una **nueva conversación** y envía el prompt estructurado:

```
[Contexto] Soy diseñador de comunicaciones internas en Contoso Corp. Necesito crear un banner digital para la intranet corporativa que acompañe el correo sobre la política de trabajo híbrido. El banner anterior (que ya tenemos) muestra personas trabajando en oficina y en casa. Ahora necesito una variante complementaria con un enfoque diferente.

[Objetivo] Genera una descripción detallada (prompt para generación de imagen con IA) que pueda usar en Microsoft Designer para crear un nuevo banner que transmita "conexión y colaboración entre equipos presenciales y remotos".

[Fuentes] La identidad visual de Contoso Corp usa: color primario azul (#0078D4), estilo moderno y minimalista, personas diversas, ambientes tecnológicos limpios. El banner será horizontal (1920x680 píxeles) para la cabecera de la intranet.

[Expectativas] La descripción debe ser un prompt listo para usar en un generador de imágenes. Debe incluir: estilo visual (flat illustration o 3D suave), composición (qué elementos y dónde), paleta de colores (azules y blancos predominantes), ambiente (profesional pero humano), y elementos simbólicos de conexión (líneas, redes, dispositivos). Máximo 80 palabras. En inglés (los generadores de imágenes funcionan mejor en inglés). Proporciona 3 variantes distintas.
```

6. Registra el prompt y la respuesta.
7. Escribe la comparación entre ambos resultados.
8. Aplica la **primera ronda de refinamiento**:

```
Refinamiento 1: De las 3 variantes, la segunda me parece más interesante. Expándela a 100 palabras agregando más detalle sobre la disposición espacial de los elementos y especificando que las personas deben verse en una videoconferencia donde algunos están en oficina y otros en casa. Mantén el estilo flat illustration.
```

9. Aplica la **segunda ronda de refinamiento**:

```
Refinamiento 2: Perfecto. Ahora genera una versión adicional de ese mismo prompt pero adaptada para formato cuadrado (1080x1080) pensada para publicación en el canal de Teams de Contoso Corp. Ajusta la composición para que funcione en formato cuadrado sin perder los elementos clave.
```

10. Registra ambos refinamientos con sus resultados en el documento.

**Resultado esperado:** El prompt COFE genera 3 descripciones detalladas y específicas en inglés, listas para usar en un generador de imágenes, con indicaciones de estilo, composición y paleta de colores alineadas con la marca de Contoso Corp. Los refinamientos producen variantes adaptadas a diferentes formatos.

**Verificación:** El Escenario 3 tiene documentados todos los prompts, resultados, comparación y dos refinamientos. Las descripciones generadas son utilizables directamente en Microsoft Designer.

---

### Paso 7: Reflexiones y cierre del catálogo

**Objetivo:** Consolidar los aprendizajes documentando patrones observados y mejores prácticas descubiertas durante el laboratorio.

**Instrucciones:**

1. En tu documento `Catalogo-Prompts-Lab03.docx`, navega a la sección **"Reflexiones y Aprendizajes"**.
2. Responde por escrito las siguientes preguntas (mínimo 2-3 oraciones por pregunta):

```
1. ¿Cuál fue la diferencia más notable entre los resultados de prompts básicos vs. estructurados?

2. ¿Qué componente del marco COFE (Contexto, Objetivo, Fuentes o Expectativas) tuvo mayor impacto en la calidad de las respuestas? ¿Por qué?

3. ¿En qué momento del refinamiento iterativo sentiste que la respuesta alcanzó calidad "lista para usar"? ¿Fue en la primera ronda, la segunda, o necesitarías más?

4. ¿Qué tipo de tarea (redacción, análisis o generación creativa) fue más fácil de estructurar con COFE? ¿Cuál fue más desafiante?

5. Escribe 3 reglas personales que seguirás al redactar prompts en el futuro.
```

3. Guarda el documento final.
4. Verifica que el archivo esté sincronizado en OneDrive revisando el ícono de estado (✓ verde) junto al archivo.

**Resultado esperado:** La sección de reflexiones contiene respuestas sustantivas que demuestran comprensión del marco COFE y capacidad de autoevaluación sobre la práctica realizada.

**Verificación:** El documento completo contiene todas las secciones llenas: 3 escenarios con prompts básicos, prompts COFE, comparaciones, refinamientos y reflexiones finales.

---

## Validación y Pruebas

Antes de considerar el laboratorio completado, verifica los siguientes criterios:

| # | Criterio de Validación | ✓ |
|---|------------------------|---|
| 1 | El archivo `Catalogo-Prompts-Lab03.docx` existe en `OneDrive\Curso-M365-Copilot\Lab03\` | ☐ |
| 2 | Los 3 escenarios tienen documentados tanto el prompt básico como el prompt COFE | ☐ |
| 3 | Los 3 escenarios tienen documentados los resultados de ambos tipos de prompt | ☐ |
| 4 | Los 3 escenarios incluyen una sección de comparación con al menos 3 diferencias observadas | ☐ |
| 5 | Cada escenario tiene al menos 2 rondas de refinamiento iterativo documentadas | ☐ |
| 6 | La sección de Reflexiones y Aprendizajes está completa con las 5 preguntas respondidas | ☐ |
| 7 | El correo final del Escenario 1 incluye: asunto ≤8 palabras, datos de Contoso, enlace al formulario, P.D. | ☐ |
| 8 | El resumen ejecutivo del Escenario 2 incluye: tabla de KPIs, recomendaciones con prioridad, responsables | ☐ |
| 9 | Las descripciones del Escenario 3 están en inglés y son utilizables en un generador de imágenes | ☐ |
| 10 | El documento está correctamente guardado y sincronizado en OneDrive (ícono ✓ verde) | ☐ |

---

## Solución de Problemas

### Problema 1: Copilot Chat no reconoce el contexto de conversaciones anteriores al refinar

**Síntomas:** Al enviar un prompt de refinamiento, Copilot responde como si no tuviera contexto previo, genera contenido completamente nuevo o pregunta "¿A qué te refieres?"

**Causa:** Se inició accidentalmente una nueva conversación (nuevo tema) en lugar de continuar en la misma sesión. Copilot Chat no mantiene contexto entre conversaciones separadas. También puede ocurrir si la sesión expiró por inactividad prolongada (más de 10-15 minutos sin interacción).

**Solución:**
1. Verifica en el panel lateral izquierdo de Copilot Chat que estás en la misma conversación donde generaste la respuesta original.
2. Si la conversación se perdió, inicia una nueva y vuelve a enviar el prompt COFE completo antes de intentar el refinamiento.
3. Para evitar este problema: realiza los refinamientos inmediatamente después del prompt inicial sin pausas prolongadas.
4. Si necesitas una pausa, copia la última respuesta de Copilot y, al retomar, pégala como contexto: "Continuando con esta respuesta que generaste anteriormente: [pegar respuesta]. Ahora necesito los siguientes ajustes..."

---

### Problema 2: Copilot genera respuestas que exceden significativamente la extensión solicitada

**Síntomas:** A pesar de especificar "máximo 300 palabras" o "máximo una página" en las expectativas, Copilot genera respuestas de 500+ palabras o múltiples páginas.

**Causa:** Copilot Chat tiende a priorizar la completitud sobre la concisión cuando el prompt incluye múltiples instrucciones detalladas. El modelo interpreta cada instrucción como un requisito que necesita desarrollo extenso, especialmente cuando se combinan datos numéricos con solicitudes de formato específico.

**Solución:**
1. Agrega la restricción de extensión como la **última línea** del prompt, separada y enfática: `IMPORTANTE: La respuesta completa NO debe exceder 300 palabras. Sé conciso.`
2. Si la respuesta ya fue generada y es demasiado larga, usa un refinamiento: `Reduce la respuesta anterior a exactamente 300 palabras o menos, manteniendo los puntos más importantes y eliminando redundancias.`
3. Alternativa: divide el prompt en dos partes. Primero genera el contenido sin restricción de extensión, luego en un segundo mensaje pide: `Condensa lo anterior en máximo 300 palabras sin perder información clave.`

---

## Limpieza

Este laboratorio no requiere eliminación de recursos ya que los archivos generados serán insumos para el Lab 03-02-01. Asegúrate de:

1. **Mantener** el archivo `Catalogo-Prompts-Lab03.docx` en `OneDrive\Curso-M365-Copilot\Lab03\` — será referencia para laboratorios posteriores.
2. **No eliminar** las conversaciones de Copilot Chat — puedes consultarlas en el historial si necesitas verificar algún resultado.
3. **Cerrar** las pestañas de Copilot Chat que ya no uses para mantener el navegador organizado.
4. **Verificar** la sincronización de OneDrive: el ícono en la barra de tareas debe mostrar estado "Actualizado" (✓).

---

## Resumen

En este laboratorio has practicado la transformación de solicitudes vagas en prompts estructurados de alta calidad usando el marco COFE. Los principales logros incluyen:

| Competencia Desarrollada | Evidencia |
|--------------------------|-----------|
| Aplicación del marco COFE | 3 prompts estructurados con los 4 componentes explícitos |
| Comparación cualitativa | 3 análisis documentados de diferencias entre prompts básicos vs. estructurados |
| Personalización por tipo de tarea | Prompts adaptados para redacción, análisis y generación creativa |
| Refinamiento iterativo | 6 rondas de refinamiento (2 por escenario) con mejoras progresivas |
| Documentación reutilizable | Catálogo completo de prompts en formato Word |

**Conexión con laboratorios posteriores:**
- El **correo final** del Escenario 1 será utilizado como contenido base en el Lab 03-02-01 (presentación en PowerPoint).
- El **resumen ejecutivo** del Escenario 2 proporcionará los datos para las diapositivas de análisis.
- Las **descripciones de imagen** del Escenario 3 podrán usarse para generar nuevos assets visuales en laboratorios del Módulo 4.

### Recursos Adicionales

- Marco COFE detallado: Revisar la lección 3.1 del curso para profundizar en cada componente
- Documento de referencia: `OneDrive\Curso-M365-Copilot\Recursos-Compartidos\Contexto-Contoso-Corp.pdf`
- Práctica adicional: Intenta aplicar el marco COFE a una tarea real de tu trabajo diario y compara resultados

---

# Práctica guiada: Crear una presentación con Copilot usando plantillas de marca y refinar el resultado

## Metadata

| Campo | Detalle |
|-------|---------|
| **Duración** | 90 minutos |
| **Complejidad** | Alta |
| **Nivel Bloom** | Aplicar |
| **Tecnologías principales** | Microsoft PowerPoint 2405 con Copilot integrado, OneDrive for Business, Plantilla .potx corporativa |
| **Escenario** | Contoso Corp — Presentación ejecutiva sobre política de trabajo híbrido |

## Descripción General

En este laboratorio crearás una presentación ejecutiva completa de 8–12 diapositivas sobre la política de trabajo híbrido de Contoso Corp utilizando Copilot en PowerPoint. Integrarás todos los recursos generados en laboratorios anteriores (imagen de banner, correo de comunicación y resumen del formulario de satisfacción) sobre la plantilla de marca corporativa. Tras la generación inicial, aplicarás al menos 5 refinamientos iterativos documentados, simulando un flujo de trabajo real de producción de contenido corporativo asistido por IA.

## Objetivos de Aprendizaje

Al completar este laboratorio serás capaz de:

- [ ] Definir contexto, objetivo, fuentes y expectativas (marco COFE) para la generación de una presentación corporativa con Copilot en PowerPoint
- [ ] Utilizar una plantilla de marca corporativa (.potx) y recursos visuales para generar una presentación visualmente consistente con la identidad de Contoso Corp
- [ ] Integrar recursos de laboratorios anteriores (imagen, texto de correo, resumen de formulario) como insumos para Copilot en PowerPoint
- [ ] Aplicar técnicas de refinamiento iterativo sobre diapositivas individuales mediante solicitudes específicas a Copilot
- [ ] Evaluar la coherencia visual y narrativa de la presentación generada y documentar las decisiones de refinamiento

## Prerrequisitos

### Conocimientos previos

| Requisito | Origen |
|-----------|--------|
| Marco COFE (Contexto, Objetivo, Fuentes, Expectativas) | Lab 03-01-01 |
| Uso básico de Copilot Chat para generar y refinar texto | Labs 01-03-01 y 03-01-01 |
| Generación de imágenes con Microsoft Designer/Copilot | Lab 02-03-01 |
| Navegación básica en PowerPoint (cinta de opciones, panel de diapositivas) | Conocimiento general |

### Archivos requeridos en OneDrive

| Archivo | Ubicación | Origen |
|---------|-----------|--------|
| `Banner-Hibrido-Final.png` | `OneDrive\Curso-M365-Copilot\Lab02\` | Lab 02-03-01 |
| `Correo-Comunicacion-Hibrido.docx` | `OneDrive\Curso-M365-Copilot\Lab03\` | Lab 03-01-01 |
| `Resumen-Formulario-Satisfaccion.docx` | `OneDrive\Curso-M365-Copilot\Lab03\` | Lab 03-01-01 |
| `Contoso-Brand-Template.potx` | `OneDrive\Curso-M365-Copilot\Recursos-Compartidos\` | Provisto por instructor |
| `Contexto-Contoso-Corp.pdf` | `OneDrive\Curso-M365-Copilot\Recursos-Compartidos\` | Provisto por instructor |

### Acceso y licencias

- Cuenta corporativa del dominio del curso (usuario@contoso-curso.onmicrosoft.com)
- Licencia Microsoft 365 Copilot activa y asignada
- Carpeta `OneDrive\Curso-M365-Copilot\Lab04\` creada y sincronizada

## Entorno del Laboratorio

### Software requerido

| Aplicación | Versión mínima | Verificación |
|------------|----------------|--------------|
| Microsoft PowerPoint | Versión 2405 (Build 17628.20144) | Archivo → Cuenta → Acerca de PowerPoint |
| OneDrive for Business | 24.071.0407.0003 | Icono de nube en barra de tareas → Configuración → Acerca de |
| Microsoft Edge | 124.0.2478.105 | edge://version |

### Verificación previa del entorno

Antes de iniciar, ejecuta estas comprobaciones:

1. Abre PowerPoint → verifica que el botón **Copilot** aparezca en la cinta de opciones (pestaña **Inicio**)
2. Navega a OneDrive en el Explorador de archivos → confirma que los 5 archivos listados en prerrequisitos existen
3. Abre `Contoso-Brand-Template.potx` haciendo doble clic → confirma que se abre una nueva presentación con los colores azul (#0078D4), blanco y gris oscuro (#323130), tipografía Segoe UI y logo de Contoso

---

## Instrucciones Paso a Paso

### Paso 1: Planificar la presentación aplicando el marco COFE

**Objetivo:** Redactar un brief estructurado que servirá como solicitud principal para Copilot en PowerPoint.

**Instrucciones:**

1. Abre el archivo `Contexto-Contoso-Corp.pdf` desde `OneDrive\Curso-M365-Copilot\Recursos-Compartidos\` y revisa los datos clave:
   - Empresa: Contoso Corp (tecnología, 500 empleados)
   - Política híbrida: 3 días presencial, 2 remoto
   - Satisfacción: 72% satisfechos, 18% neutrales, 10% insatisfechos

2. Abre el archivo `Correo-Comunicacion-Hibrido.docx` desde `OneDrive\Curso-M365-Copilot\Lab03\` y extrae los puntos clave del mensaje que se comunicará.

3. Abre el archivo `Resumen-Formulario-Satisfaccion.docx` desde `OneDrive\Curso-M365-Copilot\Lab03\` y anota los hallazgos principales de la encuesta.

4. En un archivo de texto nuevo (Bloc de notas o Word), redacta tu brief COFE siguiendo esta estructura:

```
CONTEXTO: Soy parte del equipo de Recursos Humanos de Contoso Corp, 
empresa de tecnología con 500 empleados. Presento ante la Dirección General 
los resultados de satisfacción con la política de trabajo híbrido 
(3 días presencial, 2 remoto).

OBJETIVO: Que la Dirección General comprenda los resultados de satisfacción, 
valide la política actual y apruebe 3 acciones de mejora para el segmento 
neutral e insatisfecho (28% combinado).

FUENTES: Datos de satisfacción (72% satisfechos, 18% neutrales, 10% 
insatisfechos), contenido del correo de comunicación de la política, 
y resumen del formulario de satisfacción aplicado a empleados.

EXPECTATIVAS: Presentación de 8-12 diapositivas, tono ejecutivo y profesional, 
lenguaje claro sin jerga técnica de RRHH, incluir visualización de datos 
de satisfacción, imagen de banner corporativo, y cierre con próximos pasos.
```

5. Guarda este archivo como `Brief-COFE-Presentacion.txt` en `OneDrive\Curso-M365-Copilot\Lab04\`.

**Resultado esperado:** Un documento de texto con el brief COFE completo que articula las 4 dimensiones del marco para la presentación.

**Verificación:**
- [ ] El brief incluye las 4 secciones: Contexto, Objetivo, Fuentes, Expectativas
- [ ] Los datos de satisfacción (72%, 18%, 10%) están incluidos explícitamente
- [ ] Se especifica el rango de diapositivas (8-12) y el tono (ejecutivo)
- [ ] El archivo está guardado en la carpeta Lab04

---

### Paso 2: Abrir la plantilla de marca corporativa en PowerPoint

**Objetivo:** Iniciar una nueva presentación basada en la plantilla de Contoso Corp para que Copilot genere contenido respetando la identidad visual.

**Instrucciones:**

1. Navega en el Explorador de archivos a `OneDrive\Curso-M365-Copilot\Recursos-Compartidos\`.

2. Haz doble clic en `Contoso-Brand-Template.potx`. PowerPoint se abrirá con una **nueva presentación** basada en la plantilla (no editarás la plantilla original).

3. Verifica la identidad visual de la plantilla:
   - Ve a **Diseño → Variantes → Colores**: confirma que la paleta incluye azul primario (#0078D4), blanco (#FFFFFF) y gris oscuro (#323130)
   - Ve a **Diseño → Variantes → Fuentes**: confirma que la tipografía es Segoe UI
   - Revisa la diapositiva de título: el logo de Contoso Corp debe aparecer en el encabezado

4. Explora los layouts disponibles haciendo clic en **Inicio → Nueva diapositiva → desplegable**. Confirma que existen al menos 4 layouts:
   - Portada
   - Contenido
   - Datos/Estadísticas
   - Cierre

5. Guarda inmediatamente la presentación como `Presentacion-Hibrido-Contoso.pptx` en `OneDrive\Curso-M365-Copilot\Lab04\`:
   - **Archivo → Guardar como → OneDrive → Curso-M365-Copilot → Lab04**
   - Nombre: `Presentacion-Hibrido-Contoso`
   - Tipo: Presentación de PowerPoint (.pptx)

6. Espera a que el indicador de sincronización de OneDrive muestre ✓ (guardado en la nube).

**Resultado esperado:** Un archivo `.pptx` nuevo basado en la plantilla corporativa, guardado en la ubicación correcta, con todos los elementos de marca visibles.

**Verificación:**
- [ ] El archivo se llama exactamente `Presentacion-Hibrido-Contoso.pptx`
- [ ] Está guardado en `OneDrive\Curso-M365-Copilot\Lab04\`
- [ ] La paleta de colores corporativa está activa (azul #0078D4 visible)
- [ ] La tipografía Segoe UI está configurada
- [ ] El logo de Contoso aparece en los layouts

---

### Paso 3: Generar el contenido inicial con Copilot en PowerPoint

**Objetivo:** Utilizar Copilot integrado en PowerPoint para generar el borrador completo de la presentación usando el brief COFE.

**Instrucciones:**

1. Con `Presentacion-Hibrido-Contoso.pptx` abierto, haz clic en el botón **Copilot** en la cinta de opciones (pestaña **Inicio**). Se abrirá el panel de Copilot en el lado derecho.

2. En el panel de Copilot, escribe la siguiente solicitud (adaptada de tu brief COFE). Copia y pega, ajustando si es necesario según el contenido específico de tus archivos de laboratorios anteriores:

```
Crea una presentación ejecutiva de 10 diapositivas sobre los resultados 
de satisfacción con la política de trabajo híbrido de Contoso Corp. 

Contexto: Contoso Corp es una empresa de tecnología con 500 empleados 
que implementó una política de trabajo híbrido (3 días presencial, 
2 días remoto). Se realizó una encuesta de satisfacción con estos 
resultados: 72% satisfechos, 18% neutrales, 10% insatisfechos.

Audiencia: Dirección General de Contoso Corp.

Objetivo: Presentar los resultados, validar la política actual y proponer 
3 acciones de mejora para el 28% que no está plenamente satisfecho.

Estructura solicitada:
1. Portada con título "Resultados de Satisfacción: Política de Trabajo Híbrido"
2. Agenda de la presentación
3. Contexto de la política híbrida (3 días oficina, 2 remoto)
4. Metodología de la encuesta aplicada
5. Resultados generales de satisfacción (72%, 18%, 10%)
6. Análisis del segmento neutral (18%)
7. Análisis del segmento insatisfecho (10%)
8. Propuesta de 3 acciones de mejora
9. Cronograma de implementación
10. Cierre y próximos pasos

Tono: Ejecutivo, profesional, conciso. Sin jerga técnica de RRHH.
Incluye visualizaciones de datos donde sea apropiado.
```

3. Presiona **Enter** o haz clic en el botón de enviar. Espera mientras Copilot genera las diapositivas (puede tomar 15-45 segundos).

4. Revisa el resultado generado:
   - Cuenta el número de diapositivas creadas
   - Verifica que los colores y fuentes de la plantilla corporativa se mantienen
   - Confirma que los datos de satisfacción (72%, 18%, 10%) aparecen en al menos una diapositiva
   - Observa si Copilot incluyó gráficos o visualizaciones de datos

5. Si Copilot generó menos de 8 diapositivas o el resultado no incluye la estructura solicitada, escribe en el panel:

```
Agrega las diapositivas que faltan según la estructura de 10 diapositivas 
que solicité. Asegúrate de incluir la diapositiva de propuesta de 3 acciones 
de mejora y el cronograma de implementación.
```

6. Guarda la presentación (**Ctrl + S**).

**Resultado esperado:** Una presentación de 8-12 diapositivas con contenido estructurado sobre la política híbrida, usando la paleta de colores y tipografía de la plantilla corporativa.

**Verificación:**
- [ ] La presentación tiene entre 8 y 12 diapositivas
- [ ] Los datos 72%, 18% y 10% aparecen explícitamente
- [ ] Los colores corporativos (azul #0078D4) se mantienen en todas las diapositivas
- [ ] La tipografía Segoe UI está presente en títulos y cuerpo de texto
- [ ] Existe al menos una diapositiva con propuesta de acciones de mejora
- [ ] El tono es ejecutivo y profesional

---

### Paso 4: Insertar el banner corporativo generado en el Lab 02

**Objetivo:** Integrar la imagen `Banner-Hibrido-Final.png` creada en el laboratorio anterior como recurso visual en la presentación.

**Instrucciones:**

1. Navega a la diapositiva de **portada** (diapositiva 1) en el panel de diapositivas.

2. Usa Copilot para solicitar la integración de la imagen. En el panel de Copilot, escribe:

```
En la diapositiva de portada, agrega una imagen de fondo o banner visual 
que represente el trabajo híbrido. Usa una imagen que transmita colaboración 
entre personas en oficina y en remoto.
```

3. Si Copilot no puede insertar directamente tu imagen personalizada (comportamiento esperado en la mayoría de los casos), insértala manualmente:
   - Selecciona la diapositiva 1 (portada)
   - Ve a **Insertar → Imágenes → Este dispositivo** (o **OneDrive**)
   - Navega a `OneDrive\Curso-M365-Copilot\Lab02\`
   - Selecciona `Banner-Hibrido-Final.png` → **Insertar**

4. Ajusta la imagen insertada:
   - Redimensiona para que ocupe aproximadamente el 40-50% inferior de la diapositiva, o el área de fondo según el layout de portada de la plantilla
   - Haz clic derecho sobre la imagen → **Enviar al fondo** si es necesario para que el texto del título quede visible
   - Ajusta la transparencia si el texto es difícil de leer: **Formato de imagen → Transparencia → 20-30%**

5. Verifica que el banner se integra visualmente con la paleta corporativa (azul, blanco, gris).

6. Guarda la presentación (**Ctrl + S**).

**Resultado esperado:** La diapositiva de portada muestra el banner `Banner-Hibrido-Final.png` integrado visualmente con los elementos de marca corporativa.

**Verificación:**
- [ ] La imagen `Banner-Hibrido-Final.png` está visible en la diapositiva de portada
- [ ] El título de la presentación sigue siendo legible sobre o junto a la imagen
- [ ] La composición visual es coherente con la paleta corporativa
- [ ] No hay elementos superpuestos que dificulten la lectura

---

### Paso 5: Enriquecer el contenido con información de laboratorios anteriores

**Objetivo:** Incorporar contenido del correo de comunicación y del resumen del formulario para dar profundidad y coherencia narrativa a la presentación.

**Instrucciones:**

1. Abre en una ventana separada el archivo `Correo-Comunicacion-Hibrido.docx` desde `OneDrive\Curso-M365-Copilot\Lab03\`. Identifica los puntos clave del mensaje (beneficios de la política, lineamientos, expectativas).

2. Regresa a PowerPoint. En el panel de Copilot, solicita la integración del contenido del correo:

```
En la diapositiva sobre el contexto de la política híbrida, incorpora 
los siguientes puntos clave que se comunicaron a los empleados:
- La política establece 3 días presenciales (martes, miércoles, jueves) 
  y 2 días remotos (lunes y viernes)
- Se busca equilibrar la colaboración presencial con la flexibilidad
- La empresa proporciona equipamiento para el trabajo remoto
Presenta estos puntos de forma visual con viñetas concisas.
```

3. Abre en otra ventana el archivo `Resumen-Formulario-Satisfaccion.docx` desde `OneDrive\Curso-M365-Copilot\Lab03\`. Extrae los hallazgos principales.

4. En el panel de Copilot, solicita la incorporación de los hallazgos del formulario:

```
En la diapositiva de resultados generales, presenta los datos de la encuesta 
de satisfacción de forma visual. Los datos son:
- 72% de los empleados están satisfechos con la política híbrida
- 18% se muestran neutrales (principales razones: falta de claridad 
  en horarios, desconexión con el equipo)
- 10% están insatisfechos (principales razones: preferencia por 100% 
  remoto, dificultades de desplazamiento)
- La encuesta fue respondida por 420 de 500 empleados (84% de participación)
Usa un gráfico de dona o barras para los porcentajes principales.
```

5. Revisa las diapositivas modificadas. Si Copilot no generó un gráfico visual, créalo manualmente:
   - Selecciona la diapositiva de resultados
   - **Insertar → Gráfico → Circular (dona)**
   - Ingresa los datos: Satisfechos 72, Neutrales 18, Insatisfechos 10
   - Aplica colores corporativos al gráfico (azul para satisfechos, gris para neutrales, un tono de alerta para insatisfechos)

6. Guarda la presentación (**Ctrl + S**).

**Resultado esperado:** Las diapositivas de contexto y resultados contienen información específica extraída de los documentos de laboratorios anteriores, con datos visualizados de forma clara.

**Verificación:**
- [ ] La diapositiva de contexto incluye los lineamientos de la política (días específicos)
- [ ] La diapositiva de resultados muestra los porcentajes con alguna forma de visualización (gráfico, íconos o infografía)
- [ ] La tasa de participación (84%) está mencionada
- [ ] Las razones de neutralidad e insatisfacción están documentadas en la presentación

---

### Paso 6: Realizar 5 refinamientos iterativos con Copilot

**Objetivo:** Aplicar técnicas de refinamiento específico sobre diapositivas individuales, documentando cada solicitud y su resultado.

**Instrucciones:**

Realizarás exactamente 5 refinamientos. Para cada uno, documenta en un archivo aparte la solicitud enviada, el resultado obtenido y tu evaluación.

1. Crea un nuevo documento Word y guárdalo como `Registro-Refinamientos.docx` en `OneDrive\Curso-M365-Copilot\Lab04\`. Usa la siguiente estructura para cada refinamiento:

```
REFINAMIENTO #[número]
- Diapositiva afectada: [número y título]
- Solicitud enviada a Copilot: [texto exacto]
- Resultado obtenido: [descripción breve]
- Evaluación: [Aceptado / Aceptado con ajuste manual / Rechazado y reintentado]
- Justificación: [por qué se aceptó o rechazó]
```

2. **Refinamiento #1 — Ajuste de tono en la diapositiva de propuestas:**

   En el panel de Copilot, selecciona o navega a la diapositiva de propuesta de acciones de mejora y escribe:

```
Reformula el contenido de esta diapositiva para que las 3 acciones de mejora 
suenen como recomendaciones estratégicas, no como tareas operativas. 
Usa verbos de impacto: "Implementar", "Rediseñar", "Establecer". 
Cada acción debe tener un título breve (máximo 5 palabras) y una descripción 
de una línea que explique el beneficio esperado.
```

   Documenta el resultado en `Registro-Refinamientos.docx`.

3. **Refinamiento #2 — Adición de notas del orador:**

```
Agrega notas del orador a las diapositivas 3, 5 y 8. Las notas deben incluir 
puntos de conversación adicionales que el presentador puede mencionar 
verbalmente pero que no aparecen en la diapositiva. Máximo 3 bullets 
por diapositiva en las notas.
```

   Verifica las notas haciendo clic en **Ver → Notas** o expandiendo el panel de notas en la parte inferior de cada diapositiva. Documenta.

4. **Refinamiento #3 — Mejora visual de la diapositiva de datos:**

```
En la diapositiva de resultados generales de satisfacción, mejora el diseño 
visual. Quiero que los tres porcentajes (72%, 18%, 10%) se muestren como 
números grandes y destacados, cada uno con un color diferente y un ícono 
representativo. El 72% en azul corporativo con ícono de aprobación, 
el 18% en gris con ícono de interrogación, el 10% en naranja con ícono 
de alerta.
```

   Si Copilot no puede aplicar íconos específicos, realiza el ajuste manualmente usando **Insertar → Íconos**. Documenta.

5. **Refinamiento #4 — Transiciones y coherencia narrativa:**

```
Revisa la transición narrativa entre las diapositivas 5, 6 y 7 
(resultados generales, análisis de neutrales, análisis de insatisfechos). 
Agrega una frase de transición al inicio de las diapositivas 6 y 7 
que conecte con la diapositiva anterior. Por ejemplo: "Del 28% que no 
está plenamente satisfecho, exploremos primero el segmento neutral..."
```

   Documenta.

6. **Refinamiento #5 — Fortalecimiento del cierre:**

```
Reformula la diapositiva final de cierre y próximos pasos. Debe incluir:
- Un resumen de una línea del hallazgo principal
- Las 3 acciones propuestas en formato de lista numerada
- Una fecha tentativa de seguimiento: "Próxima revisión: [mes siguiente]"
- Una frase de cierre motivacional alineada con los valores de innovación 
  y bienestar de Contoso Corp
```

   Documenta.

7. Guarda `Registro-Refinamientos.docx` y la presentación (**Ctrl + S** en ambos archivos).

**Resultado esperado:** La presentación muestra mejoras visibles en tono, estructura narrativa, diseño visual y coherencia tras los 5 refinamientos. El registro documenta cada decisión.

**Verificación:**
- [ ] Se realizaron exactamente 5 refinamientos documentados
- [ ] El archivo `Registro-Refinamientos.docx` contiene las 5 entradas completas
- [ ] Al menos 3 de los 5 refinamientos produjeron cambios visibles en la presentación
- [ ] La presentación mantiene coherencia visual (colores, fuentes) tras los refinamientos
- [ ] Las notas del orador están presentes en al menos 3 diapositivas

---

### Paso 7: Revisión final de coherencia visual y narrativa

**Objetivo:** Evaluar la presentación completa como un todo, verificando que la identidad corporativa, el flujo narrativo y la calidad del contenido cumplen estándares ejecutivos.

**Instrucciones:**

1. Activa la vista **Clasificador de diapositivas** (**Ver → Clasificador de diapositivas**) para ver todas las diapositivas en miniatura simultáneamente.

2. Realiza una inspección visual rápida verificando:
   - ¿Todas las diapositivas usan la misma paleta de colores?
   - ¿El logo de Contoso aparece consistentemente?
   - ¿La tipografía es uniforme (Segoe UI) en todas las diapositivas?
   - ¿Hay alguna diapositiva con demasiado texto o demasiado vacía?

3. Regresa a la vista **Normal**. Inicia la presentación en modo **Presentación con diapositivas** (**F5**) y recórrela completa como si fueras el presentador:
   - ¿El flujo narrativo es lógico? (contexto → datos → análisis → propuesta → cierre)
   - ¿Cada diapositiva comunica una sola idea principal?
   - ¿Los datos son legibles a primera vista?

4. Si identificas inconsistencias, usa Copilot para un ajuste final:

```
Revisa toda la presentación y verifica que el tono sea consistentemente 
ejecutivo y profesional en todas las diapositivas. Si alguna diapositiva 
tiene un tono diferente o usa lenguaje informal, reformúlala para mantener 
la coherencia.
```

5. Realiza una última verificación de los elementos de marca:
   - **Diseño → Variantes**: confirma paleta activa
   - Revisa que no haya fuentes sustituidas (busca indicadores amarillos de fuente faltante)

6. Guarda la versión final (**Ctrl + S**). Confirma que el archivo está sincronizado con OneDrive (ícono ✓ verde).

**Resultado esperado:** Una presentación pulida, coherente visual y narrativamente, lista para ser utilizada en el Lab 04-01-01 (generación de video).

**Verificación:**
- [ ] Todas las diapositivas usan la paleta corporativa sin excepciones
- [ ] La tipografía Segoe UI es consistente en toda la presentación
- [ ] El flujo narrativo sigue la estructura: contexto → datos → análisis → propuesta → cierre
- [ ] No hay diapositivas con más de 6-7 líneas de texto (principio de legibilidad)
- [ ] La presentación se reproduce sin errores en modo Presentación (F5)

---

## Validación y Pruebas

Completa la siguiente lista de verificación final para confirmar que el laboratorio se ha completado exitosamente:

| # | Criterio | Estado |
|---|----------|--------|
| 1 | `Brief-COFE-Presentacion.txt` existe en `Lab04\` con las 4 dimensiones COFE | ☐ |
| 2 | `Presentacion-Hibrido-Contoso.pptx` existe en `Lab04\` | ☐ |
| 3 | La presentación tiene entre 8 y 12 diapositivas | ☐ |
| 4 | La plantilla corporativa está aplicada (colores, fuentes, logo) | ☐ |
| 5 | `Banner-Hibrido-Final.png` está insertado en la diapositiva de portada | ☐ |
| 6 | Los datos de satisfacción (72%, 18%, 10%) aparecen con visualización | ☐ |
| 7 | Contenido del correo de comunicación está integrado | ☐ |
| 8 | Contenido del resumen del formulario está integrado | ☐ |
| 9 | `Registro-Refinamientos.docx` existe en `Lab04\` con 5 entradas completas | ☐ |
| 10 | Notas del orador presentes en al menos 3 diapositivas | ☐ |
| 11 | La presentación pasa la revisión de coherencia visual (Paso 7) | ☐ |
| 12 | Todos los archivos están sincronizados con OneDrive (✓ verde) | ☐ |

**Criterio de éxito:** 10 de 12 criterios cumplidos = laboratorio completado satisfactoriamente. Los 12 criterios = desempeño sobresaliente.

---

## Solución de Problemas

### Problema 1: Copilot no aparece en la cinta de opciones de PowerPoint

**Síntomas:** Al abrir PowerPoint, no se ve el botón "Copilot" en la pestaña Inicio. El panel lateral de Copilot no está disponible.

**Causa:** La licencia de Microsoft 365 Copilot no está asignada correctamente a la cuenta del participante, o la versión de PowerPoint es anterior a la requerida (2405, Build 17628.20144).

**Solución:**
1. Verifica la versión: **Archivo → Cuenta → Acerca de PowerPoint**. Si es anterior a 2405, actualiza: **Archivo → Cuenta → Opciones de actualización → Actualizar ahora**.
2. Cierra y reabre PowerPoint tras la actualización.
3. Si la versión es correcta pero Copilot no aparece, cierra sesión de la cuenta Microsoft 365 (**Archivo → Cuenta → Cerrar sesión**) y vuelve a iniciar sesión con la cuenta corporativa del curso.
4. Si persiste, notifica al instructor para verificar la asignación de licencia Copilot en el portal de administración de Microsoft 365.

---

### Problema 2: Copilot genera la presentación sin respetar los colores/fuentes de la plantilla

**Síntomas:** Tras enviar la solicitud a Copilot, las diapositivas generadas usan colores genéricos (azul predeterminado de Office, fuente Calibri) en lugar de la paleta corporativa de Contoso (azul #0078D4, Segoe UI).

**Causa:** La plantilla `.potx` no se cargó correctamente antes de invocar a Copilot, o Copilot aplicó un tema predeterminado al generar contenido nuevo que sobreescribió los estilos de la plantilla.

**Solución:**
1. Ve a **Diseño → Temas**. Verifica si el tema activo es el de Contoso Corp.
2. Si no lo es, haz clic en **Diseño → desplegable de Temas → Buscar temas** y selecciona nuevamente `Contoso-Brand-Template.potx` desde OneDrive.
3. Aplica el tema a todas las diapositivas: **clic derecho sobre el tema → Aplicar a todas las diapositivas**.
4. Para futuros intentos, asegúrate de guardar el archivo `.pptx` basado en la plantilla **antes** de invocar a Copilot (como se indica en el Paso 2).
5. Si los colores del gráfico no se actualizan automáticamente, selecciona el gráfico → **Diseño de gráfico → Cambiar colores** → selecciona la paleta que coincida con los colores corporativos.

---

## Limpieza

Al finalizar el laboratorio, verifica que tu carpeta `OneDrive\Curso-M365-Copilot\Lab04\` contenga únicamente los siguientes archivos generados:

| Archivo | Propósito |
|---------|-----------|
| `Brief-COFE-Presentacion.txt` | Planificación con marco COFE |
| `Presentacion-Hibrido-Contoso.pptx` | Presentación final (se usará en Lab 04-01-01) |
| `Registro-Refinamientos.docx` | Documentación de los 5 refinamientos |

**No elimines** ninguno de estos archivos, ya que `Presentacion-Hibrido-Contoso.pptx` será insumo directo para el siguiente laboratorio (Lab 04-01-01: generación de video con Clipchamp).

Cierra las ventanas de los archivos de referencia (`Correo-Comunicacion-Hibrido.docx`, `Resumen-Formulario-Satisfaccion.docx`, `Contexto-Contoso-Corp.pdf`) que abriste durante el laboratorio. No modifiques estos archivos fuente.

---

## Resumen

En este laboratorio aplicaste un flujo de trabajo completo de creación de presentaciones corporativas asistidas por IA:

1. **Planificación estructurada** con el marco COFE antes de interactuar con Copilot
2. **Uso de plantilla de marca** para garantizar coherencia visual desde el primer borrador
3. **Generación inicial** con una solicitud detallada que integra contexto, audiencia, objetivo y estructura
4. **Integración de recursos previos** (imagen, textos de laboratorios anteriores) para crear un producto cohesivo
5. **Refinamiento iterativo** documentado (5 ciclos) que demuestra que el valor de Copilot se maximiza con interacción deliberada
6. **Evaluación holística** de coherencia visual y narrativa como paso final de calidad

### Conceptos clave reforzados

- El marco COFE reduce significativamente la necesidad de correcciones posteriores
- Partir de una plantilla corporativa antes de invocar a Copilot produce mejores resultados que aplicar el tema después
- Los refinamientos específicos (por diapositiva, con instrucciones claras) son más efectivos que solicitudes genéricas de "mejorar"
- La documentación de decisiones de refinamiento desarrolla criterio profesional para el uso de IA generativa

### Conexión con el siguiente laboratorio

El archivo `Presentacion-Hibrido-Contoso.pptx` será el insumo principal del **Lab 04-01-01**, donde generarás un video narrado a partir de esta presentación usando Microsoft Clipchamp integrado en Microsoft 365.

### Recursos adicionales

- [Usar Copilot en PowerPoint - Soporte Microsoft](https://support.microsoft.com/es-es/copilot-powerpoint)
- [Crear y guardar una plantilla de PowerPoint](https://support.microsoft.com/es-es/office/crear-y-guardar-una-plantilla-de-powerpoint)
- [Guía de Brand Kit en Microsoft Designer](https://designer.microsoft.com)

---
