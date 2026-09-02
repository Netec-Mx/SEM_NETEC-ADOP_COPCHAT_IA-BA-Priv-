# Práctica guiada: Solicitar a Copilot la creación de un formulario a partir de una necesidad definida

## Metadatos

| Campo | Detalle |
|-------|---------|
| **Duración** | 50 minutos |
| **Complejidad** | Fácil |
| **Nivel de Bloom** | Aplicar |
| **Tecnologías** | Microsoft 365 Copilot Chat (copilot.microsoft.com), Microsoft Forms (forms.office.com), Microsoft Edge 124.0.2478.105, OneDrive for Business |

## Descripción General

En este laboratorio traducirás una necesidad organizacional concreta —la recopilación de opiniones sobre la política de trabajo híbrido de Contoso Corp— en un formulario funcional creado con la asistencia de Microsoft 365 Copilot Chat. Seguirás un flujo de trabajo completo: definición de la necesidad con el modelo PACT, redacción de un prompt estructurado, refinamiento iterativo de las preguntas propuestas por Copilot, y construcción final del formulario en Microsoft Forms. El formulario resultante será el insumo base para los laboratorios posteriores del curso.

## Objetivos de Aprendizaje

Al finalizar este laboratorio serás capaz de:

- [ ] Identificar una necesidad de recopilación de información y traducirla en una solicitud estructurada para Copilot usando el modelo PACT (Propósito, Audiencia, Condiciones, Tono).
- [ ] Utilizar Microsoft 365 Copilot Chat para generar preguntas relevantes que den forma a un formulario de satisfacción laboral.
- [ ] Refinar las propuestas de Copilot mediante al menos dos solicitudes de seguimiento que mejoren la calidad y pertinencia de las preguntas.
- [ ] Construir un formulario funcional en Microsoft Forms basado en las preguntas generadas y validar su estructura antes de publicarlo.

## Prerrequisitos

### Conocimientos previos

| Requisito | Descripción |
|-----------|-------------|
| Navegación web básica | Saber abrir sitios web, iniciar sesión y navegar entre pestañas en Microsoft Edge |
| Manejo de archivos | Crear carpetas y guardar documentos en OneDrive |
| Lectura del escenario | Haber leído el documento `Contexto-Contoso-Corp.pdf` ubicado en `OneDrive\Curso-M365-Copilot\Recursos-Compartidos\` |

### Acceso y configuración previa

| Elemento | Verificación |
|----------|-------------|
| Cuenta corporativa Microsoft 365 | Inicio de sesión exitoso en `portal.office.com` con cuenta `@contoso-curso.onmicrosoft.com` |
| Licencia Copilot for Microsoft 365 | Asignada por el administrador del tenant |
| Copilot Chat con protección comercial | Acceso a `copilot.microsoft.com` mostrando el mensaje *"Tu organización tiene protección de datos comerciales activada"* |
| Microsoft Forms | Acceso a `forms.office.com` con permisos de creación |
| Carpeta de trabajo | Carpeta `OneDrive\Curso-M365-Copilot\Lab01\` creada y sincronizada |

## Entorno del Laboratorio

### Hardware mínimo

| Componente | Especificación |
|------------|---------------|
| Procesador | Intel Core i5 8.ª generación o AMD Ryzen 5 3000 (64 bits) |
| RAM | 8 GB mínimo |
| Almacenamiento libre | 2 GB |
| Conexión a Internet | 10 Mbps de bajada mínimo |
| Periféricos | Teclado y ratón funcionales |

### Software requerido

| Aplicación | Versión / Acceso |
|------------|-----------------|
| Microsoft Edge | 124.0.2478.105 o superior |
| Microsoft 365 Copilot Chat | Servicio web en `copilot.microsoft.com` |
| Microsoft Forms | Servicio web en `forms.office.com` |
| OneDrive for Business | Cliente de escritorio 24.071.0407.0003 o acceso web |

### Configuración inicial

Antes de comenzar, ejecuta estas verificaciones:

1. Abre Microsoft Edge y navega a `https://copilot.microsoft.com`.
2. Inicia sesión con tu cuenta corporativa `usuario@contoso-curso.onmicrosoft.com`.
3. Confirma que en la parte inferior de la interfaz aparece el texto: **"Tu organización tiene protección de datos comerciales activada"** (o equivalente en inglés: *"Your organization's data protection is on"*).
4. En una nueva pestaña, navega a `https://forms.office.com` y confirma que puedes ver el botón **+ Nuevo formulario**.
5. En otra pestaña, navega a `https://onedrive.com` y confirma que existe la carpeta `Curso-M365-Copilot\Lab01\`.

> ⚠️ **Importante:** Si no ves el mensaje de protección de datos comerciales en Copilot Chat, **no continúes**. Notifica al instructor para verificar tu asignación de licencia.

---

## Procedimiento Paso a Paso

### Paso 1: Definir la necesidad usando el modelo PACT

**Objetivo:** Estructurar la necesidad de recopilación de información de Contoso Corp antes de interactuar con Copilot.

**Instrucciones:**

1. Abre el archivo `Contexto-Contoso-Corp.pdf` desde `OneDrive\Curso-M365-Copilot\Recursos-Compartidos\`. Lee el escenario completo (empresa de tecnología, 500 empleados, política híbrida 3 días presencial / 2 remoto, datos de satisfacción: 72% satisfechos, 18% neutrales, 10% insatisfechos).

2. Abre un documento nuevo en tu editor de texto preferido o directamente en un archivo de Word en línea. Guárdalo como `PACT-Definicion.docx` en `OneDrive\Curso-M365-Copilot\Lab01\`.

3. Completa la siguiente plantilla PACT con la información del escenario de Contoso Corp:

```
MODELO PACT - Definición de Necesidad
======================================

P - Propósito:
¿Para qué se usará la información recopilada?
[Tu respuesta aquí]

A - Audiencia:
¿Quién responderá el formulario? ¿Cuántas personas? ¿Qué características tienen?
[Tu respuesta aquí]

C - Condiciones:
¿Qué restricciones existen? (anonimato, número de preguntas, idioma, tiempo estimado)
[Tu respuesta aquí]

T - Tono:
¿Cómo debe sentirse el formulario para quien lo responde?
[Tu respuesta aquí]
```

4. Completa cada campo con base en el escenario. Un ejemplo de respuesta correcta sería:

   - **Propósito:** Evaluar la satisfacción de los empleados con la nueva política de trabajo híbrido para identificar áreas de mejora y tomar decisiones informadas sobre ajustes a la política.
   - **Audiencia:** 500 colaboradores de Contoso Corp, todas las áreas y niveles jerárquicos, familiarizados con herramientas digitales.
   - **Condiciones:** Formulario anónimo, máximo 10 preguntas, en español, tiempo de respuesta no mayor a 5 minutos, incluir preguntas de escala y al menos una pregunta abierta.
   - **Tono:** Profesional pero cercano, que transmita que la opinión del colaborador es valorada.

5. Guarda el archivo.

**Resultado esperado:** Un documento `PACT-Definicion.docx` guardado en `OneDrive\Curso-M365-Copilot\Lab01\` con los cuatro campos del modelo PACT completados de forma coherente con el escenario de Contoso Corp.

**Verificación:** Revisa que tu definición incluya al menos: el objetivo específico (ajustar política híbrida), la audiencia (500 empleados), al menos 3 condiciones explícitas y una descripción del tono deseado.

---

### Paso 2: Redactar y enviar la primera solicitud a Copilot Chat

**Objetivo:** Formular un prompt estructurado que incluya contexto, objetivo, restricciones y expectativas claras para que Copilot proponga preguntas candidatas para el formulario.

**Instrucciones:**

1. Navega a `https://copilot.microsoft.com` en Microsoft Edge. Asegúrate de estar en una conversación nueva (haz clic en **Nuevo chat** si hay conversaciones previas).

2. Redacta tu primer prompt usando la información del modelo PACT que completaste en el Paso 1. Escribe el siguiente texto en el campo de chat (puedes adaptarlo ligeramente, pero mantén la estructura):

```
Actúa como un especialista en diseño de encuestas organizacionales.

Contexto: Soy parte del equipo de Recursos Humanos de Contoso Corp,
una empresa de tecnología con 500 empleados. Hace tres meses
implementamos una política de trabajo híbrido (3 días presenciales,
2 días remotos). Datos preliminares indican que el 72% de los
empleados están satisfechos, el 18% son neutrales y el 10% están
insatisfechos.

Objetivo: Necesito crear un formulario de satisfacción para
recopilar información detallada sobre la experiencia de los
empleados con esta política híbrida. Los resultados se usarán
para identificar áreas de mejora y tomar decisiones sobre
ajustes a la política antes de fin de trimestre.

Condiciones:
- El formulario debe ser anónimo
- Máximo 10 preguntas
- Incluir variedad de tipos: escala Likert (1-5), opción múltiple
  y al menos una pregunta de respuesta abierta
- Idioma: español
- Tiempo estimado de respuesta: no más de 5 minutos

Tono: Profesional pero cercano, que transmita que la opinión
del colaborador es valorada por la organización.

Por favor, propón una lista de 12 a 15 preguntas candidatas
que cubran los temas más relevantes. Para cada pregunta, indica
entre paréntesis el tipo de pregunta sugerido.
```

3. Presiona **Enter** o haz clic en el botón de enviar para enviar la solicitud.

4. Espera a que Copilot genere su respuesta completa. Lee la lista de preguntas propuestas con atención.

5. **Copia la respuesta completa de Copilot** (selecciona todo el texto de la respuesta, haz clic derecho > Copiar, o usa Ctrl+C). Pega esta respuesta en un nuevo documento de Word y guárdalo como `Respuesta-Copilot-01.docx` en `OneDrive\Curso-M365-Copilot\Lab01\`.

**Resultado esperado:** Copilot devuelve una lista de 12 a 15 preguntas candidatas organizadas por tema, con indicación del tipo de pregunta (escala, opción múltiple, respuesta abierta). Las preguntas deben ser relevantes al contexto de trabajo híbrido y estar redactadas en español con tono profesional y cercano.

**Verificación:**
- [ ] La respuesta contiene al menos 12 preguntas.
- [ ] Hay al menos 3 tipos diferentes de pregunta (escala, opción múltiple, abierta).
- [ ] Las preguntas están en español.
- [ ] El contenido es relevante al escenario de trabajo híbrido de Contoso Corp.
- [ ] El archivo `Respuesta-Copilot-01.docx` está guardado en la carpeta Lab01.

---

### Paso 3: Refinar las preguntas con una segunda solicitud

**Objetivo:** Evaluar críticamente las preguntas propuestas por Copilot y solicitar ajustes específicos para mejorar la calidad, relevancia y adecuación del formulario.

**Instrucciones:**

1. Revisa la lista de preguntas que Copilot generó en el Paso 2. Identifica al menos **tres aspectos a mejorar**. Considera los siguientes criterios:
   - ¿Hay preguntas redundantes que midan lo mismo?
   - ¿Falta algún tema importante (por ejemplo: comunicación con el equipo, herramientas tecnológicas, bienestar)?
   - ¿Alguna pregunta podría comprometer el anonimato?
   - ¿El orden es lógico (de lo general a lo específico)?
   - ¿Se respeta el límite de 10 preguntas finales?

2. En la **misma conversación** de Copilot Chat (no abras un chat nuevo), escribe tu segunda solicitud de refinamiento. Usa una estructura como la siguiente (adapta según lo que hayas identificado):

```
Gracias por las propuestas. Necesito los siguientes ajustes:

1. Reduce la lista a exactamente 10 preguntas finales,
   priorizando las que aporten información más accionable
   para la toma de decisiones.

2. Elimina cualquier pregunta que pueda comprometer el
   anonimato (como identificar el área o departamento
   específico del empleado).

3. Asegúrate de incluir al menos una pregunta sobre la
   calidad de las herramientas tecnológicas disponibles
   para el trabajo remoto.

4. Agrega una pregunta sobre la comunicación con el líder
   directo en el contexto híbrido.

5. Ordena las preguntas de lo más general (satisfacción
   global) a lo más específico (sugerencias de mejora),
   terminando con la pregunta abierta.

6. Para cada pregunta, indica las opciones de respuesta
   exactas que debería incluir el formulario.
```

3. Envía la solicitud y espera la respuesta completa de Copilot.

4. Lee la nueva lista refinada. Verifica que Copilot haya aplicado todos los cambios solicitados.

5. Copia la respuesta y pégala en un nuevo documento guardado como `Respuesta-Copilot-02.docx` en `OneDrive\Curso-M365-Copilot\Lab01\`.

**Resultado esperado:** Copilot devuelve una lista de exactamente 10 preguntas, ordenadas de lo general a lo específico, con opciones de respuesta detalladas para cada una, sin preguntas que comprometan el anonimato, y con cobertura de los temas solicitados (herramientas tecnológicas, comunicación con líder).

**Verificación:**
- [ ] La lista contiene exactamente 10 preguntas.
- [ ] No hay preguntas que identifiquen el área o departamento del respondente.
- [ ] Existe al menos una pregunta sobre herramientas tecnológicas.
- [ ] Existe al menos una pregunta sobre comunicación con el líder directo.
- [ ] Las preguntas están ordenadas de lo general a lo específico.
- [ ] Cada pregunta incluye las opciones de respuesta específicas.
- [ ] La última pregunta es de respuesta abierta.

---

### Paso 4: Realizar un tercer refinamiento de tono y formato

**Objetivo:** Solicitar un ajuste final de redacción para garantizar que el lenguaje sea inclusivo, claro y alineado con el tono corporativo de Contoso Corp.

**Instrucciones:**

1. En la **misma conversación** de Copilot Chat, envía una tercera solicitud:

```
Excelente. Ahora realiza los siguientes ajustes finales de
redacción:

1. Usa lenguaje inclusivo en todas las preguntas (evita
   masculino genérico, usa formas neutras como "colaboradores"
   en lugar de "los empleados").

2. Agrega una breve introducción para el formulario (2-3
   oraciones) que explique el propósito de la encuesta y
   asegure al respondente que sus respuestas son anónimas
   y confidenciales.

3. Agrega un mensaje de cierre (1-2 oraciones) que agradezca
   la participación.

4. Presenta el resultado final en un formato de tabla con las
   columnas: Número, Pregunta, Tipo, Opciones de respuesta.
```

2. Envía la solicitud y espera la respuesta.

3. Revisa que la tabla incluya la introducción, las 10 preguntas con sus opciones y el mensaje de cierre.

4. Copia la respuesta completa y guárdala como `Respuesta-Copilot-03-Final.docx` en `OneDrive\Curso-M365-Copilot\Lab01\`.

**Resultado esperado:** Una tabla formateada con 10 preguntas numeradas, cada una con su tipo y opciones de respuesta, precedida por un texto introductorio y seguida por un mensaje de agradecimiento. El lenguaje es inclusivo y el tono profesional pero cercano.

**Verificación:**
- [ ] La respuesta incluye un texto introductorio de 2-3 oraciones.
- [ ] Las 10 preguntas están presentadas en formato de tabla.
- [ ] El lenguaje es inclusivo (sin masculino genérico).
- [ ] Incluye un mensaje de cierre con agradecimiento.
- [ ] El archivo `Respuesta-Copilot-03-Final.docx` está guardado.

---

### Paso 5: Crear el formulario en Microsoft Forms

**Objetivo:** Trasladar las preguntas refinadas con Copilot a un formulario funcional en Microsoft Forms, configurando correctamente cada tipo de pregunta.

**Instrucciones:**

1. Abre una nueva pestaña en Microsoft Edge y navega a `https://forms.office.com`.

2. Haz clic en **+ Nuevo formulario**.

3. En el campo de título, escribe: **Encuesta de Satisfacción - Política de Trabajo Híbrido - Contoso Corp**

4. En el campo de descripción, pega el texto introductorio que Copilot generó en el Paso 4 (las 2-3 oraciones que explican el propósito y garantizan el anonimato).

5. Comienza a agregar las preguntas una por una, usando la tabla final del Paso 4 como referencia:

   **Para preguntas de escala Likert (1-5):**
   - Haz clic en **+ Agregar nuevo** > selecciona **Clasificación** (Rating).
   - Escribe el texto de la pregunta.
   - Configura la escala de 1 a 5.
   - Agrega etiquetas a los extremos (por ejemplo: 1 = "Muy insatisfecho/a", 5 = "Muy satisfecho/a").

   **Para preguntas de opción múltiple:**
   - Haz clic en **+ Agregar nuevo** > selecciona **Opción** (Choice).
   - Escribe el texto de la pregunta.
   - Agrega cada opción de respuesta en los campos correspondientes.
   - Si aplica, activa la opción **"Agregar opción 'Otro'"** para permitir respuestas personalizadas.

   **Para preguntas de respuesta abierta:**
   - Haz clic en **+ Agregar nuevo** > selecciona **Texto** (Text).
   - Escribe el texto de la pregunta.
   - Activa la opción **"Respuesta larga"** para permitir respuestas extensas.

6. Después de agregar las 10 preguntas, agrega una última sección o texto que contenga el mensaje de cierre/agradecimiento. Para esto:
   - Haz clic en **+ Agregar nuevo** > selecciona **Sección**.
   - En el título de la sección, escribe el mensaje de agradecimiento generado por Copilot.

7. Configura las opciones del formulario:
   - Haz clic en los **tres puntos (⋯)** en la esquina superior derecha > **Configuración**.
   - Verifica que **"Registrar nombre"** esté **desactivado** (para garantizar anonimato).
   - Activa **"Una respuesta por persona"** si lo deseas (opcional según contexto).
   - Configura una fecha de inicio y fin si aplica.

8. Haz clic en **Vista previa** (ícono de ojo) para revisar cómo se verá el formulario para los respondentes. Navega por todas las preguntas verificando:
   - Que el texto sea legible y sin errores.
   - Que las opciones de respuesta sean correctas.
   - Que los tipos de pregunta correspondan a lo planeado.

**Resultado esperado:** Un formulario funcional en Microsoft Forms con título, descripción introductoria, 10 preguntas correctamente configuradas (con variedad de tipos), y un mensaje de cierre. El formulario está configurado como anónimo.

**Verificación:**
- [ ] El formulario tiene título descriptivo que menciona "Contoso Corp" y "Trabajo Híbrido".
- [ ] La descripción incluye el texto introductorio sobre propósito y anonimato.
- [ ] Hay exactamente 10 preguntas agregadas.
- [ ] Hay al menos 3 preguntas de tipo escala/clasificación.
- [ ] Hay al menos 3 preguntas de tipo opción múltiple.
- [ ] Hay al menos 1 pregunta de tipo texto (respuesta abierta).
- [ ] El registro de nombre está desactivado (anonimato).
- [ ] La vista previa muestra el formulario correctamente.

---

### Paso 6: Documentar el formulario y guardar evidencias

**Objetivo:** Crear un registro documental del formulario generado para referencia en laboratorios futuros y guardar todas las evidencias del proceso.

**Instrucciones:**

1. Regresa a la vista de edición del formulario en Forms.

2. Crea un documento de Word que sirva como versión texto del formulario:
   - Abre Word en línea (`https://www.office.com` > Word > Documento en blanco).
   - Titula el documento: **"Formulario de Satisfacción - Trabajo Híbrido - Contoso Corp (Versión Texto)"**.
   - Copia el contenido completo del formulario en el documento con el siguiente formato:

```
FORMULARIO DE SATISFACCIÓN - POLÍTICA DE TRABAJO HÍBRIDO
Contoso Corp
=========================================================

INTRODUCCIÓN:
[Pega aquí el texto introductorio]

PREGUNTAS:

1. [Texto de la pregunta 1]
   Tipo: [Escala / Opción múltiple / Respuesta abierta]
   Opciones: [Lista de opciones si aplica]

2. [Texto de la pregunta 2]
   Tipo: [...]
   Opciones: [...]

[... continuar con las 10 preguntas ...]

MENSAJE DE CIERRE:
[Pega aquí el mensaje de agradecimiento]

=========================================================
Generado con asistencia de Microsoft 365 Copilot Chat
Fecha: [Fecha actual]
Laboratorio: 01-03-01
```

3. Guarda el documento como `Formulario-Satisfaccion-Hibrido.docx` en `OneDrive\Curso-M365-Copilot\Lab01\`.

4. Verifica que tu carpeta `OneDrive\Curso-M365-Copilot\Lab01\` contenga los siguientes archivos:
   - `PACT-Definicion.docx`
   - `Respuesta-Copilot-01.docx`
   - `Respuesta-Copilot-02.docx`
   - `Respuesta-Copilot-03-Final.docx`
   - `Formulario-Satisfaccion-Hibrido.docx`

5. (Opcional) Toma una captura de pantalla de tu formulario en vista previa en Forms y guárdala como `Captura-Formulario-Forms.png` en la misma carpeta.

**Resultado esperado:** Cinco documentos guardados en la carpeta Lab01 que documentan todo el proceso desde la definición de la necesidad hasta el formulario final, más el formulario publicado en Microsoft Forms.

**Verificación:**
- [ ] Los 5 archivos están presentes en `OneDrive\Curso-M365-Copilot\Lab01\`.
- [ ] El archivo `Formulario-Satisfaccion-Hibrido.docx` contiene las 10 preguntas con sus tipos y opciones.
- [ ] El formulario en Microsoft Forms está accesible y funcional (se puede abrir desde el panel de Forms).

---

## Validación y Prueba Final

Para confirmar que el laboratorio se completó exitosamente, realiza las siguientes verificaciones:

### Lista de verificación final

| # | Criterio | ✓/✗ |
|---|----------|-----|
| 1 | El modelo PACT está documentado con los 4 componentes completos | |
| 2 | Se realizaron al menos 3 interacciones con Copilot Chat (solicitud inicial + 2 refinamientos) | |
| 3 | Las respuestas de Copilot están documentadas en archivos separados | |
| 4 | El formulario en Microsoft Forms tiene exactamente 10 preguntas | |
| 5 | El formulario incluye variedad de tipos de pregunta (escala, opción múltiple, abierta) | |
| 6 | El formulario está configurado como anónimo | |
| 7 | El documento `Formulario-Satisfaccion-Hibrido.docx` está guardado en Lab01 | |
| 8 | El formulario es funcional (se puede responder desde vista previa) | |

### Prueba de funcionalidad

1. En Microsoft Forms, haz clic en **Vista previa**.
2. Responde todas las preguntas del formulario como si fueras un empleado de Contoso Corp.
3. Haz clic en **Enviar**.
4. Verifica que aparezca el mensaje de confirmación de envío.
5. Regresa a la vista de edición y haz clic en la pestaña **Respuestas** para confirmar que se registró 1 respuesta.

> ✅ Si puedes ver 1 respuesta registrada, tu formulario está completamente funcional y el laboratorio está terminado.

---

## Solución de Problemas

### Problema 1: Copilot genera respuestas en inglés en lugar de español

**Síntomas:** A pesar de escribir el prompt en español, Copilot responde parcial o totalmente en inglés. Las preguntas propuestas están en inglés o mezclan ambos idiomas.

**Causa:** La configuración regional de la cuenta de Microsoft 365 o del navegador puede estar establecida en inglés, lo que influye en el idioma predeterminado de las respuestas de Copilot. También puede ocurrir si el prompt no especifica explícitamente el idioma de salida.

**Solución:**
1. Agrega al inicio de tu próximo mensaje en la conversación: `"Por favor, responde exclusivamente en español. Todas las preguntas y opciones de respuesta deben estar redactadas en español."`
2. Verifica la configuración de idioma de tu cuenta: navega a `https://myaccount.microsoft.com/settingsandprivacy/language` y confirma que el idioma preferido sea **Español**.
3. En Microsoft Edge, ve a **Configuración > Idiomas** y asegúrate de que "Español" esté en la lista de idiomas preferidos y en primera posición.
4. Si el problema persiste, inicia un nuevo chat y agrega `Idioma de respuesta: español` como primera línea de tu prompt.

---

### Problema 2: Microsoft Forms no muestra la opción de "Clasificación" (Rating) para preguntas de escala

**Síntomas:** Al hacer clic en **+ Agregar nuevo** en Microsoft Forms, no aparece la opción "Clasificación" o "Rating" entre los tipos de pregunta disponibles. Solo se ven opciones como Opción, Texto, Fecha y Clasificación por estrellas.

**Causa:** La interfaz de Microsoft Forms puede variar según la versión del tenant y la configuración regional. En algunos tenants, la opción de escala numérica se presenta como "Clasificación" (con estrellas o números) y en otros como "Likert" (disponible solo dentro de secciones). Además, la escala Likert completa solo está disponible cuando se agrega como tipo especial.

**Solución:**
1. Para escala Likert completa: haz clic en **+ Agregar nuevo** > busca **"Likert"** en los tipos de pregunta (puede aparecer al hacer clic en los tres puntos **⋯** o en **"Más tipos de preguntas"**).
2. Si no encuentras "Likert": usa el tipo **"Clasificación"** (Rating) que permite configurar una escala numérica de 1 a 5 o de 1 a 10 con etiquetas personalizadas en los extremos.
3. Alternativa: usa una pregunta de **"Opción"** (Choice) con las opciones escritas manualmente: "1 - Muy insatisfecho/a", "2 - Insatisfecho/a", "3 - Neutral", "4 - Satisfecho/a", "5 - Muy satisfecho/a".
4. Verifica que tu cuenta tenga permisos completos de creación en Forms navegando a `https://admin.microsoft.com` > Centro de administración > Forms y confirmando que la creación de formularios está habilitada para tu usuario.

---

## Limpieza

Al finalizar el laboratorio:

1. **No elimines** el formulario de Microsoft Forms ni los archivos de la carpeta Lab01. Estos serán utilizados como insumos en los laboratorios posteriores del curso (Lab02 en adelante).

2. **Cierra las conversaciones de Copilot Chat** si no las necesitas para referencia futura, pero considera mantenerlas abiertas durante la sesión por si necesitas consultarlas.

3. **Verifica la sincronización de OneDrive:** Confirma que el ícono de OneDrive en la barra de tareas muestra una marca de verificación verde (✓), indicando que todos los archivos están sincronizados con la nube.

4. Si realizaste la prueba de funcionalidad (responder el formulario como prueba), puedes eliminar esa respuesta de prueba desde la pestaña **Respuestas** en Forms haciendo clic en los tres puntos > **Eliminar todas las respuestas**, solo si deseas que el formulario esté limpio para uso futuro.

---

## Resumen

En este laboratorio completaste el ciclo completo de creación de un formulario asistido por IA:

| Fase | Actividad realizada | Archivo generado |
|------|-------------------|-----------------|
| Definición | Estructuración de la necesidad con modelo PACT | `PACT-Definicion.docx` |
| Generación | Primera solicitud a Copilot con prompt estructurado | `Respuesta-Copilot-01.docx` |
| Refinamiento 1 | Ajustes de contenido, eliminación de redundancias | `Respuesta-Copilot-02.docx` |
| Refinamiento 2 | Ajustes de tono, formato y lenguaje inclusivo | `Respuesta-Copilot-03-Final.docx` |
| Construcción | Creación del formulario funcional en Microsoft Forms | Formulario en Forms |
| Documentación | Registro textual del formulario completo | `Formulario-Satisfaccion-Hibrido.docx` |

### Conceptos clave aplicados

- **Modelo PACT:** Propósito, Audiencia, Condiciones y Tono como estructura para definir necesidades antes de interactuar con IA.
- **Prompting estructurado:** Incluir contexto, objetivo, restricciones y formato de salida esperado en cada solicitud a Copilot.
- **Refinamiento iterativo:** Usar la misma conversación para ajustar progresivamente las propuestas de Copilot sin perder contexto.
- **Evaluación crítica:** No aceptar la primera respuesta de Copilot sin revisarla; siempre validar pertinencia, redundancia y adecuación.

### Conexión con laboratorios posteriores

El formulario creado en este laboratorio y el escenario de Contoso Corp serán reutilizados en:
- **Lab 02:** Generación de imágenes relacionadas con la comunicación del programa de trabajo híbrido.
- **Lab 03:** Creación de un catálogo de prompts y documentos de análisis basados en los datos de satisfacción.
- **Lab 04:** Presentación ejecutiva en PowerPoint con los resultados del formulario.
- **Lab 05:** Video de comunicación interna sobre los hallazgos.

### Recursos adicionales

- [Documentación oficial de Microsoft Forms](https://support.microsoft.com/es-es/forms)
- [Guía de prompts efectivos para Microsoft 365 Copilot](https://adoption.microsoft.com/es-es/copilot/)
- [Mejores prácticas para diseño de encuestas organizacionales](https://learn.microsoft.com/es-es/microsoft-forms/best-practices)

---
