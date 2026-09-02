# Práctica guiada: Generar y refinar un video corto de comunicación interna con Copilot Chat

## Metadata

| Campo | Detalle |
|-------|---------|
| **Duración** | 50 minutos |
| **Complejidad** | Media |
| **Nivel Bloom** | Aplicar |
| **Tecnologías** | Microsoft Clipchamp (app.clipchamp.com), Microsoft Copilot Chat (copilot.microsoft.com), Microsoft Edge 124+, OneDrive for Business |
| **Formato de salida** | MP4 (H.264, 1080p, máx. 90 segundos) |

---

## Descripción General

En este laboratorio generarás un video corto de comunicación interna para Contoso Corp que anuncia los resultados de la encuesta de satisfacción sobre trabajo híbrido y los próximos pasos de la política. Aplicarás el marco COFE para redactar un brief de video estructurado en Copilot Chat, producirás el video en Clipchamp con asistencia de Copilot, realizarás al menos dos refinamientos iterativos y exportarás el producto final. Este laboratorio cierra el ciclo completo del batch, integrando los outputs de todos los laboratorios anteriores como insumos.

---

## Objetivos de Aprendizaje

Al finalizar este laboratorio, serás capaz de:

- [ ] Definir con precisión el propósito, audiencia y mensaje principal de un video de comunicación interna para Contoso Corp
- [ ] Redactar un brief/guion estructurado para generación de video usando el marco COFE en Copilot Chat
- [ ] Generar un video corto (máximo 90 segundos) utilizando Copilot integrado en Clipchamp
- [ ] Aplicar al menos dos opciones de refinamiento al video generado (narración, duración, elementos visuales o música)
- [ ] Evaluar el video final según el propósito comunicativo y documentar aprendizajes sobre posibilidades y limitaciones

---

## Prerrequisitos

### Conocimiento previo

| Requisito | Fuente |
|-----------|--------|
| Marco COFE (Contexto, Objetivo, Fuentes, Expectativas) | Laboratorios 01–04 del batch |
| Experiencia en refinamiento iterativo de prompts | Labs 03-01-01 y 03-02-01 |
| Familiaridad con la interfaz de Copilot Chat empresarial | Labs anteriores |
| Datos del escenario Contoso Corp (72% satisfechos, 18% neutrales, 10% insatisfechos) | Contexto-Contoso-Corp.pdf |

### Archivos requeridos en OneDrive

| Archivo | Ubicación | Origen |
|---------|-----------|--------|
| `Presentacion-Hibrido-Contoso.pptx` | `OneDrive\Curso-M365-Copilot\Lab04\` | Lab 03-02-01 |
| `Banner-Hibrido-Final.png` | `OneDrive\Curso-M365-Copilot\Lab02\` | Lab 02-03-01 |
| `Correo-Comunicacion-Hibrido.docx` | `OneDrive\Curso-M365-Copilot\Lab03\` | Lab 03-01-01 |
| `Contexto-Contoso-Corp.pdf` | `OneDrive\Curso-M365-Copilot\Recursos-Compartidos\` | Proporcionado por instructor |

### Acceso verificado

- [ ] Cuenta corporativa del dominio del curso activa (usuario@contoso-curso.onmicrosoft.com)
- [ ] Licencia Copilot for Microsoft 365 asignada
- [ ] Acceso a `copilot.microsoft.com` con protección de datos comerciales visible
- [ ] Acceso a `app.clipchamp.com` con la función Copilot habilitada
- [ ] Carpeta `OneDrive\Curso-M365-Copilot\Lab05\` creada

---

## Entorno del Laboratorio

### Hardware mínimo

| Componente | Especificación |
|------------|---------------|
| Procesador | Intel Core i5 8ª gen. / AMD Ryzen 5 3000 o superior (64 bits) |
| RAM | 8 GB mínimo (16 GB recomendado) |
| Almacenamiento libre | 2 GB mínimo |
| Internet | 10 Mbps descarga / 5 Mbps subida |
| Periféricos | Micrófono y altavoces/auriculares (recomendado) |

### Software requerido

| Aplicación | Versión / Acceso |
|------------|-----------------|
| Microsoft Edge | 124.0.2478.105 o superior |
| Microsoft Clipchamp | Versión 2.8.0 — acceso vía `app.clipchamp.com` |
| Microsoft Copilot Chat | `copilot.microsoft.com` — servicio en la nube |
| OneDrive for Business | Cliente de escritorio sincronizado (24.071+) |

### Verificación inicial del entorno

1. Abre Microsoft Edge y navega a `copilot.microsoft.com`.
2. Confirma que aparece el mensaje: **"Tu organización tiene protección de datos comerciales activada"**.
3. En una nueva pestaña, navega a `app.clipchamp.com` e inicia sesión con tu cuenta corporativa.
4. Verifica que en la pantalla principal de Clipchamp aparezca la opción **"Crear un video con IA"** o **"Create with AI"**.
5. Abre el Explorador de archivos y confirma que la carpeta `OneDrive\Curso-M365-Copilot\Lab05\` existe y está sincronizada (ícono de nube con check verde).

> ⚠️ **Si no ves la protección de datos comerciales en Copilot Chat o no aparece la opción de IA en Clipchamp, detente y notifica al instructor antes de continuar.**

---

## Procedimiento Paso a Paso

### Paso 1: Revisión de insumos y definición del brief creativo

**Objetivo:** Consolidar la información de laboratorios anteriores para definir el propósito, audiencia y mensaje principal del video.

**Instrucciones:**

1. Abre los siguientes archivos desde OneDrive para revisar su contenido (no es necesario editarlos):
   - `Lab04\Presentacion-Hibrido-Contoso.pptx` — identifica los mensajes clave y datos estadísticos
   - `Lab03\Correo-Comunicacion-Hibrido.docx` — observa el tono de comunicación utilizado
   - `Lab02\Banner-Hibrido-Final.png` — nota los elementos visuales de marca

2. En un documento nuevo o en un bloc de notas, completa el siguiente brief creativo basándote en el escenario de Contoso Corp:

   | Campo | Tu definición |
   |-------|---------------|
   | **Propósito** | Informar resultados de la encuesta de satisfacción y anunciar próximos pasos de la política híbrida |
   | **Audiencia** | Todos los colaboradores de Contoso Corp (500 empleados, perfiles administrativos y técnicos) |
   | **Mensaje principal** | "Los resultados de nuestra encuesta confirman que el modelo híbrido funciona: 72% de satisfacción. Ahora evolucionamos juntos hacia la siguiente fase." |
   | **Duración** | Máximo 90 segundos |
   | **Tono** | Profesional, positivo, cercano y transparente |
   | **Llamado a la acción** | Revisar los próximos pasos en la intranet y participar en la siguiente ronda de retroalimentación |

3. Guarda este brief como referencia para el siguiente paso. Puedes mantenerlo en un archivo de texto o simplemente tenerlo visible en pantalla.

**Resultado esperado:** Un brief creativo completo con los seis campos definidos, basado en datos reales del escenario Contoso Corp.

**Verificación:** Confirma que tu mensaje principal incluye el dato de 72% de satisfacción y que el propósito combina "informar resultados" con "anunciar próximos pasos".

---

### Paso 2: Generación del guion y storyboard en Copilot Chat

**Objetivo:** Utilizar Copilot Chat con el marco COFE para generar un guion de video estructurado y un storyboard textual.

**Instrucciones:**

1. Navega a `copilot.microsoft.com` en Microsoft Edge.

2. Ingresa el siguiente prompt, adaptando si lo deseas con tus propias palabras pero manteniendo la estructura COFE:

```
Actúa como guionista de comunicación interna corporativa.

CONTEXTO: Soy parte del equipo de comunicaciones de Contoso Corp, una empresa 
de tecnología con 500 empleados. Acabamos de completar una encuesta de 
satisfacción sobre nuestra política de trabajo híbrido (3 días presencial, 
2 días remoto). Los resultados son: 72% satisfechos, 18% neutrales y 10% 
insatisfechos. Necesito crear un video de comunicación interna para compartir 
estos resultados con todos los colaboradores.

OBJETIVO: Generar un guion de locución y un storyboard textual para un video 
de máximo 90 segundos que informe los resultados de la encuesta y anuncie los 
próximos pasos de la política híbrida.

FUENTES: 
- Datos de la encuesta: 72% satisfechos, 18% neutrales, 10% insatisfechos
- Tono de referencia: profesional, positivo, cercano y transparente
- Identidad visual: paleta azul corporativo (#0078D4), blanco y gris oscuro
- Próximos pasos: ajustes en días flexibles, nuevas herramientas de 
  colaboración remota, segunda ronda de retroalimentación en 3 meses

EXPECTATIVAS:
- Formato: tabla con columnas Segmento | Tiempo | Locución | Visual sugerido | 
  Texto en pantalla
- Dividir en 5 segmentos de 15-20 segundos cada uno
- Incluir apertura con gancho, presentación de datos, próximos pasos, 
  llamado a la acción y cierre con identidad corporativa
- Sugerir estilo de música de fondo al final
- El tono de la locución debe ser como si un líder cercano hablara directamente 
  a su equipo
```

3. Revisa la respuesta de Copilot. Verifica que contenga:
   - Una tabla con 5 segmentos claramente definidos
   - Tiempos que sumen aproximadamente 75-90 segundos
   - Mención explícita del dato de 72% de satisfacción
   - Un llamado a la acción claro en el segmento 4 o 5
   - Sugerencia de estilo musical

4. Si la respuesta no cumple con algún criterio, realiza un refinamiento. Ejemplo de prompt de seguimiento:

```
El segmento 3 es demasiado genérico. Reescríbelo incluyendo los tres datos 
específicos de la encuesta (72%, 18%, 10%) y presentándolos de forma visual 
progresiva. Además, el cierre necesita ser más memorable: sugiere un slogan 
corto de máximo 6 palabras para Contoso Corp sobre trabajo híbrido.
```

5. Copia el guion final aprobado y guárdalo en un archivo llamado `Guion-Video-Hibrido.txt` en la carpeta `OneDrive\Curso-M365-Copilot\Lab05\`.

**Resultado esperado:** Un guion completo en formato de tabla con 5 segmentos, tiempos definidos, locución detallada, descripciones visuales y texto en pantalla. Ejemplo de estructura esperada:

| Segmento | Tiempo | Locución | Visual sugerido | Texto en pantalla |
|----------|--------|----------|-----------------|-------------------|
| 1 - Apertura | 0:00–0:15 | "En Contoso creemos que la mejor forma de trabajar es la que diseñamos juntos..." | Personas colaborando en oficina y desde casa | Logo Contoso Corp |
| 2 - Datos | 0:15–0:35 | "Escuchamos sus voces: 72% de ustedes están satisfechos con nuestro modelo híbrido..." | Gráfica animada con porcentajes | "72% satisfechos · 18% neutrales · 10% insatisfechos" |
| 3 - Próximos pasos | 0:35–0:55 | "Estos resultados nos impulsan a mejorar..." | Íconos de flexibilidad, herramientas, feedback | "Más flexibilidad · Mejores herramientas · Tu voz cuenta" |
| 4 - CTA | 0:55–1:15 | "Visita la intranet para conocer el plan completo..." | Pantalla de intranet simulada | "Consulta los próximos pasos en la intranet" |
| 5 - Cierre | 1:15–1:30 | "Contoso Corp. Juntos, mejor." | Logo sobre fondo azul corporativo | "Juntos, mejor." |

**Verificación:** El archivo `Guion-Video-Hibrido.txt` existe en `Lab05\` y contiene una tabla completa con 5 segmentos que suman entre 75 y 90 segundos.

---

### Paso 3: Generación del video en Clipchamp con Copilot

**Objetivo:** Producir el video inicial utilizando Clipchamp con asistencia de Copilot, basándose en el guion generado.

**Instrucciones:**

1. Navega a `app.clipchamp.com` e inicia sesión con tu cuenta corporativa.

2. En la pantalla principal, selecciona **"Crear un video con IA"** (o "Create a video with AI" si la interfaz está en inglés).

3. Cuando Copilot solicite una descripción del video, ingresa el siguiente texto basado en tu brief y guion:

```
Crea un video de comunicación interna corporativa de 60-90 segundos para 
Contoso Corp, una empresa de tecnología. El video anuncia los resultados 
de una encuesta de satisfacción sobre trabajo híbrido: 72% satisfechos, 
18% neutrales, 10% insatisfechos. 

El tono debe ser profesional y positivo. Incluye:
- Apertura con personas trabajando en oficina y desde casa
- Sección de datos con los porcentajes de satisfacción
- Próximos pasos: más flexibilidad, mejores herramientas, nueva ronda de 
  retroalimentación
- Llamado a la acción: visitar la intranet
- Cierre con identidad corporativa

Estilo visual: corporativo moderno, colores azul y blanco.
Incluir texto en pantalla con los datos clave.
Música de fondo: corporativa, optimista, no intrusiva.
```

4. Selecciona las opciones de personalización que Clipchamp ofrezca:
   - **Estilo/Tema:** Corporativo o Profesional
   - **Relación de aspecto:** 16:9 (horizontal/widescreen)
   - **Duración:** 60-90 segundos (si permite seleccionar)

5. Haz clic en **"Generar"** o **"Create"** y espera a que Clipchamp produzca el borrador del video (esto puede tomar 30-60 segundos).

6. Una vez generado, reproduce el video completo en el editor de Clipchamp para evaluarlo. Toma nota de:
   - ¿La duración es adecuada (≤ 90 segundos)?
   - ¿Los clips visuales son coherentes con el tema de trabajo híbrido?
   - ¿El texto en pantalla es legible y correcto?
   - ¿La música es apropiada para el tono deseado?
   - ¿Hay narración automática? ¿El ritmo es adecuado?

**Resultado esperado:** Un borrador de video en el timeline de Clipchamp con clips de stock, texto en pantalla, transiciones y música de fondo. El video debe estar entre 60 y 90 segundos de duración.

**Verificación:** El video se reproduce sin errores en el editor de Clipchamp, muestra contenido relacionado con el entorno laboral y contiene al menos un elemento de texto en pantalla con datos de la encuesta.

---

### Paso 4: Primer refinamiento — Ajuste de narración y texto en pantalla

**Objetivo:** Aplicar el primer ciclo de refinamiento modificando la narración (voz en off o texto) y corrigiendo los textos en pantalla para alinearlos con el guion aprobado.

**Instrucciones:**

1. En el editor de Clipchamp, identifica la pista de **texto en pantalla** (text overlays) en el timeline.

2. Haz doble clic en cada elemento de texto y modifícalo para que coincida con el guion del Paso 2:
   - Segmento 1: Agrega o edita para mostrar "Contoso Corp" con el logo (si es posible importar `Banner-Hibrido-Final.png`)
   - Segmento 2: Asegura que muestre "72% satisfechos · 18% neutrales · 10% insatisfechos"
   - Segmento 3: Edita para mostrar "Más flexibilidad · Mejores herramientas · Tu voz cuenta"
   - Segmento 4: Confirma que el CTA diga "Consulta los próximos pasos en la intranet"
   - Segmento 5: Edita el cierre para mostrar "Juntos, mejor."

3. Para la narración, selecciona una de estas opciones según la disponibilidad en tu versión de Clipchamp:

   **Opción A — Texto a voz (Text-to-Speech):**
   - Selecciona **"Grabar y crear" > "Texto a voz"** en el panel izquierdo
   - Copia el texto de locución del Segmento 1 de tu guion
   - Selecciona un idioma: **Español (México)** o **Español (España)**
   - Selecciona una voz que suene profesional y cercana
   - Genera el audio y arrástralo al timeline en la posición correspondiente
   - Repite para cada segmento

   **Opción B — Grabación de voz propia (si tienes micrófono):**
   - Selecciona **"Grabar y crear" > "Audio"**
   - Lee en voz alta el texto de locución del guion
   - Ajusta el volumen y la posición en el timeline

   **Opción C — Sin narración de voz:**
   - Si las opciones anteriores no están disponibles, refuerza el texto en pantalla para que sea autoexplicativo
   - Aumenta el tamaño de fuente y la duración de cada texto

4. Reproduce el video completo para verificar la sincronización entre la narración y los elementos visuales.

**Resultado esperado:** El video ahora muestra textos en pantalla alineados con el guion oficial de Contoso Corp y cuenta con narración (automática o grabada) que sigue el script del Paso 2.

**Verificación:** Al reproducir el video, los textos en pantalla coinciden con los mensajes del guion y la narración (si existe) es audible y está sincronizada con las transiciones visuales.

---

### Paso 5: Segundo refinamiento — Ajuste de elementos visuales y música

**Objetivo:** Aplicar el segundo ciclo de refinamiento modificando clips visuales, importando la imagen de marca y ajustando la música de fondo.

**Instrucciones:**

1. **Importar imagen de marca:**
   - En el panel izquierdo de Clipchamp, selecciona **"Tus medios"** o **"Importar medios"**
   - Navega a `OneDrive\Curso-M365-Copilot\Lab02\` y selecciona `Banner-Hibrido-Final.png`
   - Arrastra la imagen al timeline en el segmento de apertura o cierre (como overlay o como clip de fondo durante 3-5 segundos)

2. **Reemplazar clips visuales no relevantes:**
   - Revisa cada clip de stock en el timeline
   - Si algún clip no es coherente con el tema (por ejemplo, muestra una industria diferente a tecnología), haz clic derecho y selecciona **"Reemplazar"** o busca un nuevo clip en la biblioteca de stock
   - Usa términos de búsqueda como: "hybrid work", "office technology", "remote collaboration", "team meeting"

3. **Ajustar música de fondo:**
   - En el panel izquierdo, selecciona **"Música y efectos de sonido"**
   - Busca pistas con etiquetas como: "corporate", "uplifting", "positive", "inspiring"
   - Selecciona una pista que sea suave y no compita con la narración
   - Ajusta el volumen de la música al **20-30%** del volumen total para que la narración sea protagonista
   - Recorta la pista musical para que coincida con la duración total del video

4. **Ajustar transiciones:**
   - Entre cada segmento, verifica que exista una transición suave
   - Si hay cortes bruscos, agrega transiciones tipo "Fade" o "Dissolve" de 0.5 segundos

5. Reproduce el video completo una vez más. Evalúa:
   - ¿La imagen `Banner-Hibrido-Final.png` es visible y está bien posicionada?
   - ¿Los clips visuales reflejan un entorno de trabajo híbrido en tecnología?
   - ¿La música complementa sin distraer?
   - ¿Las transiciones son fluidas?

**Resultado esperado:** Un video refinado que incorpora la identidad visual de Contoso Corp (banner del Lab 02), clips de stock relevantes al tema de trabajo híbrido, música corporativa apropiada y transiciones suaves.

**Verificación:** El video contiene al menos un elemento visual propio (Banner-Hibrido-Final.png), la música de fondo es audible pero no domina sobre la narración/texto, y no hay cortes abruptos entre segmentos.

---

### Paso 6: Exportación del video final

**Objetivo:** Exportar el video en formato MP4 a resolución 1080p y guardarlo en la carpeta designada de OneDrive.

**Instrucciones:**

1. Reproduce el video una última vez de inicio a fin para confirmar que estás satisfecho con el resultado.

2. Verifica la duración total en el timeline: debe ser **≤ 90 segundos**.

3. Haz clic en el botón **"Exportar"** (esquina superior derecha de Clipchamp).

4. Selecciona la calidad de exportación: **1080p (Full HD)**.

5. Espera a que el proceso de exportación finalice (puede tomar 1-3 minutos dependiendo de la duración y los elementos del video).

6. Una vez completada la exportación, Clipchamp ofrecerá opciones para guardar:
   - Selecciona **"Guardar en OneDrive"** si la opción está disponible
   - Alternativamente, descarga el archivo y muévelo manualmente

7. Renombra el archivo como: `Video-Comunicacion-Hibrido-Final.mp4`

8. Ubica el archivo en: `OneDrive\Curso-M365-Copilot\Lab05\`

9. Confirma que el archivo se sincroniza correctamente (ícono de check verde en OneDrive).

**Resultado esperado:** Un archivo MP4 de máximo 90 segundos, resolución 1080p, guardado correctamente en la carpeta Lab05 de OneDrive.

**Verificación:**
- El archivo `Video-Comunicacion-Hibrido-Final.mp4` existe en `OneDrive\Curso-M365-Copilot\Lab05\`
- El tamaño del archivo es razonable (típicamente entre 15-80 MB para un video de 60-90 segundos en 1080p)
- El archivo se reproduce correctamente al hacer doble clic desde el Explorador de archivos

---

### Paso 7: Reflexión documentada y evaluación del proceso

**Objetivo:** Evaluar el video final en función del propósito comunicativo y documentar aprendizajes sobre el flujo completo del batch.

**Instrucciones:**

1. Navega a `copilot.microsoft.com` y utiliza el siguiente prompt para generar una estructura de reflexión:

```
Ayúdame a crear una plantilla de reflexión profesional sobre un proceso de 
creación de video con IA. La plantilla debe tener las siguientes secciones:

1. Evaluación del video final (¿cumple el propósito comunicativo?)
2. Efectividad del marco COFE en la generación de video
3. Comparación: primer borrador vs. versión final (¿qué mejoró con los 
   refinamientos?)
4. Conexión con laboratorios anteriores (¿cómo los outputs previos 
   enriquecieron este video?)
5. Posibilidades y limitaciones de la generación de video con IA
6. Tres aprendizajes clave del batch completo

Formato: documento con encabezados y espacio para respuestas de 2-3 oraciones 
por sección.
```

2. Copia la plantilla generada por Copilot en un nuevo documento.

3. Completa cada sección con tus propias observaciones. Puntos guía:

   **Sección 1 — Evaluación del video:**
   - ¿El video comunica claramente que 72% de los empleados están satisfechos?
   - ¿El llamado a la acción es claro?
   - ¿Un colaborador de Contoso entendería el mensaje en una sola visualización?

   **Sección 2 — Marco COFE:**
   - ¿Definir Contexto, Objetivo, Fuentes y Expectativas antes de generar mejoró la calidad?
   - ¿Qué componente del marco fue más útil para este tipo de contenido?

   **Sección 3 — Refinamientos:**
   - ¿Cuántos ciclos de refinamiento realizaste?
   - ¿Qué cambió más significativamente entre el borrador inicial y la versión final?

   **Sección 4 — Conexión con labs anteriores:**
   - ¿Cómo influyó el banner del Lab 02 en la identidad visual del video?
   - ¿El tono del correo del Lab 03 se reflejó en la narración?
   - ¿Los datos de la presentación del Lab 04 se comunicaron efectivamente?

   **Sección 5 — Posibilidades y limitaciones:**
   - ¿Qué puede hacer bien la IA generativa en video?
   - ¿Qué requiere todavía intervención humana significativa?
   - ¿Qué no pudo hacer la herramienta que hubieras deseado?

   **Sección 6 — Tres aprendizajes clave:**
   - Sintetiza en tres frases los aprendizajes más importantes del batch completo (Labs 01-05)

4. Guarda el documento como `Reflexion-Final-Lab05.docx` en `OneDrive\Curso-M365-Copilot\Lab05\`.

**Resultado esperado:** Un documento de reflexión de 1-2 páginas con observaciones personales sobre el proceso, las herramientas y los aprendizajes del batch.

**Verificación:** El archivo `Reflexion-Final-Lab05.docx` existe en la carpeta `Lab05\` y contiene respuestas sustantivas en las 6 secciones (no está vacío ni tiene solo la plantilla sin completar).

---

## Validación y Pruebas Finales

Antes de dar por completado el laboratorio, verifica los siguientes entregables en `OneDrive\Curso-M365-Copilot\Lab05\`:

| # | Entregable | Criterio de aceptación |
|---|-----------|----------------------|
| 1 | `Guion-Video-Hibrido.txt` | Contiene tabla con 5 segmentos, tiempos definidos, locución y descripciones visuales |
| 2 | `Video-Comunicacion-Hibrido-Final.mp4` | Formato MP4, resolución 1080p, duración ≤ 90 segundos, se reproduce sin errores |
| 3 | `Reflexion-Final-Lab05.docx` | 6 secciones completadas con observaciones personales |

### Lista de verificación de calidad del video

- [ ] El video dura 90 segundos o menos
- [ ] Se mencionan o muestran los datos de la encuesta (72%, 18%, 10%)
- [ ] Existe un llamado a la acción visible/audible
- [ ] Se incorporó al menos un elemento visual propio (Banner-Hibrido-Final.png)
- [ ] La música de fondo no compite con la narración/texto
- [ ] Se aplicaron al menos 2 refinamientos documentables respecto al borrador inicial
- [ ] El tono es profesional, positivo y coherente con la comunicación de Contoso Corp

---

## Solución de Problemas

### Problema 1: La opción "Crear con IA" no aparece en Clipchamp

**Síntomas:** Al acceder a `app.clipchamp.com`, la pantalla principal muestra opciones de creación manual pero no el botón de generación con IA/Copilot.

**Causa:** La funcionalidad de Copilot en Clipchamp requiere que la licencia Copilot for Microsoft 365 esté correctamente asignada al usuario Y que el administrador del tenant haya habilitado las funcionalidades de IA en Clipchamp. En algunos tenants, esta función puede estar en despliegue gradual.

**Solución:**
1. Cierra sesión en Clipchamp y vuelve a iniciar sesión con tu cuenta corporativa.
2. Verifica tu licencia en `myaccount.microsoft.com` > Suscripciones.
3. Si la función sigue sin aparecer, utiliza el **flujo alternativo**:
   - Crea el video manualmente en Clipchamp usando el guion del Paso 2 como guía
   - Selecciona "Crear nuevo video" > elige plantilla "Corporate" o "Business"
   - Agrega clips de stock manualmente buscando por términos relevantes
   - Inserta los textos en pantalla manualmente según el storyboard
   - Agrega narración con texto-a-voz o grabación propia
   - Este flujo alternativo cumple los mismos objetivos de aprendizaje
4. Notifica al instructor para que verifique la configuración del tenant.

---

### Problema 2: El video exportado excede los 90 segundos de duración

**Síntomas:** Tras la exportación, el archivo MP4 tiene una duración de 100-120 segundos, superando el límite requerido de 90 segundos.

**Causa:** Clipchamp con Copilot puede generar contenido más extenso de lo solicitado, especialmente si el prompt de generación incluye muchos elementos. Las transiciones y los silencios entre segmentos también agregan tiempo inadvertidamente.

**Solución:**
1. Regresa al editor de Clipchamp (el proyecto se guarda automáticamente).
2. En el timeline, identifica el marcador de tiempo 1:30 (90 segundos).
3. Selecciona todo el contenido posterior a 1:30 y elimínalo.
4. Alternativas para reducir duración sin perder contenido:
   - Reduce la duración de los clips de cada segmento (arrastra los bordes en el timeline)
   - Elimina pausas o silencios entre segmentos
   - Fusiona los segmentos 4 (CTA) y 5 (Cierre) en uno solo de 15 segundos
   - Acelera ligeramente la velocidad de narración si usaste texto-a-voz (velocidad 1.1x)
5. Reproduce para confirmar que el contenido sigue siendo coherente.
6. Exporta nuevamente en 1080p y reemplaza el archivo anterior.

---

## Limpieza

Este es el último laboratorio del batch, por lo que no se requiere eliminar archivos. Sin embargo, asegúrate de:

1. **Cerrar sesión** en Clipchamp (`app.clipchamp.com` > ícono de perfil > Cerrar sesión).
2. **Verificar la sincronización** completa de OneDrive: confirma que todos los archivos de `Lab05\` muestran el ícono de check verde.
3. **Estructura final de carpetas** — Confirma que tu directorio completo del curso contiene:

```
OneDrive\Curso-M365-Copilot\
├── Lab01\          (formulario y prompts)
├── Lab02\          (Banner-Hibrido-Final.png y otras imágenes)
├── Lab03\          (Correo-Comunicacion-Hibrido.docx y catálogo de prompts)
├── Lab04\          (Presentacion-Hibrido-Contoso.pptx y registro de refinamientos)
├── Lab05\          ← ESTE LABORATORIO
│   ├── Guion-Video-Hibrido.txt
│   ├── Video-Comunicacion-Hibrido-Final.mp4
│   └── Reflexion-Final-Lab05.docx
└── Recursos-Compartidos\
    ├── Contexto-Contoso-Corp.pdf
    └── Contoso-Brand-Template.potx
```

4. Si el instructor lo solicita, comparte la carpeta `Lab05\` con permisos de lectura para evaluación.

---

## Resumen

En este laboratorio completaste el ciclo final del batch, transformando una idea de comunicación interna en un video corporativo funcional mediante las siguientes etapas:

| Etapa | Herramienta | Producto |
|-------|-------------|----------|
| Planificación (Brief creativo) | Revisión de labs anteriores | Brief con propósito, audiencia, mensaje, tono y CTA |
| Guionización | Copilot Chat + marco COFE | Guion de 5 segmentos con storyboard textual |
| Producción | Clipchamp con Copilot | Borrador de video con clips, texto y música |
| Refinamiento 1 | Clipchamp (editor manual) | Narración y textos alineados al guion |
| Refinamiento 2 | Clipchamp (editor manual) | Imagen de marca, clips relevantes, música ajustada |
| Exportación | Clipchamp | MP4 1080p ≤ 90 segundos |
| Reflexión | Copilot Chat + redacción propia | Documento de aprendizajes |

### Conceptos clave consolidados en este laboratorio

- **El brief creativo es el prompt más importante:** La calidad del video depende directamente de la claridad con la que defines propósito, audiencia y mensaje antes de interactuar con la IA.
- **El refinamiento iterativo es indispensable:** La IA genera un punto de partida, no un producto final. El valor humano está en evaluar, ajustar y mejorar.
- **Los outputs se encadenan:** El banner del Lab 02, el tono del Lab 03 y los datos del Lab 04 enriquecieron directamente este video, demostrando el poder de los flujos de trabajo encadenados con IA.
- **Posibilidades y limitaciones coexisten:** La IA puede generar estructura, seleccionar recursos y acelerar la producción, pero el juicio editorial, la coherencia de marca y la conexión emocional siguen requiriendo intervención humana.

### Recursos adicionales

- [Documentación oficial de Clipchamp](https://support.microsoft.com/clipchamp)
- [Guía de Copilot en Microsoft 365](https://support.microsoft.com/copilot)
- [Mejores prácticas de comunicación interna en video](https://learn.microsoft.com/microsoft-365/community/)
- [Marco COFE — Referencia rápida del curso](OneDrive\Curso-M365-Copilot\Recursos-Compartidos\)

---

# Práctica guiada: Usar Planner Agent para generar un plan de trabajo a partir de una descripción de necesidad

## Metadatos

| Campo | Valor |
|---|---|
| **Duración** | 35 minutos |
| **Complejidad** | Fácil |
| **Nivel Bloom** | Aplicar |
| **Tecnologías** | Microsoft 365 Copilot Chat, Planner Agent, Microsoft Planner (New Planner), OneDrive, Word Online |

## Descripción General

En este laboratorio asumirás el rol de coordinador de operaciones de la empresa ficticia **Distribuidora Andina S.A.** Tu tarea es generar un plan de trabajo completo para una auditoría interna de procesos administrativos programada en 8 semanas. Utilizarás **Planner Agent** dentro de Copilot Chat para transformar una descripción de necesidad en un plan estructurado con 4 etapas, tareas específicas y fechas asignadas, refinándolo iterativamente hasta obtener un resultado de calidad ejecutiva que guardarás en Microsoft Planner y exportarás a OneDrive.

## Objetivos de Aprendizaje

Al completar este laboratorio serás capaz de:

- [ ] Identificar y activar Planner Agent dentro de Copilot Chat en Microsoft 365
- [ ] Formular un prompt inicial estructurado (marco NECT) que describa una necesidad organizacional concreta para generar un plan de trabajo
- [ ] Organizar el plan resultante en 4 etapas lógicas con al menos 3 tareas por etapa y fechas tentativas
- [ ] Refinar el plan mediante prompts de seguimiento para agregar tareas, ajustar fechas y asignar responsables ficticios
- [ ] Guardar el plan en Microsoft Planner y exportar un resumen en texto a OneDrive para uso en laboratorios posteriores

## Prerrequisitos

### Conocimientos Previos

| Conocimiento | Nivel |
|---|---|
| Navegación en el portal de Microsoft 365 | Básico |
| Uso de Copilot Chat (escribir prompts y leer respuestas) | Básico |
| Concepto de plan de trabajo (etapas, tareas, fechas) | Básico |
| Gestión de archivos en OneDrive | Básico |

### Acceso y Configuración Previa

- Cuenta corporativa Microsoft 365 con licencia **Microsoft 365 Copilot** asignada
- Acceso verificado a Copilot Chat en `https://microsoft365.com/copilot` o en Microsoft Teams
- Microsoft Planner (New Planner) habilitado en el tenant
- Carpeta **`Copilot_Labs`** creada previamente en OneDrive
- Protección de datos comerciales activa (verificar mensaje en Copilot Chat)

## Entorno del Laboratorio

### Software Requerido

| Aplicación | Versión / Acceso |
|---|---|
| Microsoft Edge o Google Chrome | Edge 124+ o Chrome 124+ |
| Microsoft 365 Copilot Chat | `https://microsoft365.com/copilot` (servicio en la nube) |
| Planner Agent | Integrado en Copilot Chat (activación con `@Planner`) |
| Microsoft Planner | New Planner — acceso vía portal Microsoft 365 |
| Microsoft Word Online | Acceso vía OneDrive (build 2405) |
| OneDrive for Business | Versión web |

### Verificación Inicial del Entorno

Antes de iniciar, confirma lo siguiente:

1. Abre `https://microsoft365.com/copilot` en tu navegador.
2. Verifica que aparezca el mensaje **"Tu organización tiene protección de datos comerciales activada"** (o equivalente en inglés: *"Your organization's data protection is on"*).
3. Abre una nueva pestaña y navega a `https://tasks.office.com` para confirmar acceso a Microsoft Planner.
4. Abre otra pestaña y navega a tu OneDrive (`https://onedrive.com`). Confirma que existe la carpeta **`Copilot_Labs`**.

> ⚠️ **IMPORTANTE**: Si no ves el mensaje de protección de datos comerciales en Copilot Chat, NO continúes. Notifica al instructor para verificar tu licencia.

---

## Paso 1: Acceder a Copilot Chat e Identificar Planner Agent

### Objetivo
Navegar a Copilot Chat y confirmar que Planner Agent está disponible como agente especializado.

### Instrucciones

1. Abre **Microsoft Edge** (o Google Chrome) y navega a:
   ```
   https://microsoft365.com/copilot
   ```

2. Inicia sesión con tu cuenta corporativa del curso (ej. `usuario@contoso-curso.onmicrosoft.com`).

3. Una vez en la interfaz de Copilot Chat, localiza el **campo de texto** de entrada de mensajes en la parte inferior de la pantalla.

4. En el campo de texto, escribe el símbolo `@` (arroba). Esto desplegará una lista de **agentes disponibles**.

5. En la lista desplegable, busca y selecciona **"Planner"** (puede aparecer como "Microsoft Planner" o con el ícono de Planner — un cuadrado verde con una marca de verificación).

6. Una vez seleccionado, verás que en el campo de texto aparece `@Planner` seguido de un espacio, indicando que el agente está activo para tu próximo mensaje.

7. **No escribas nada aún.** Simplemente confirma que el agente se activó correctamente.

### Resultado Esperado

- La interfaz de Copilot Chat muestra `@Planner` en el campo de texto con un indicador visual (ícono o etiqueta) que confirma la selección del agente.
- No hay mensajes de error ni advertencias sobre permisos.

### Verificación

| Criterio | ✓ / ✗ |
|---|---|
| Copilot Chat cargó correctamente con protección de datos comerciales | |
| El símbolo `@` despliega la lista de agentes disponibles | |
| "Planner" aparece en la lista y se puede seleccionar | |
| `@Planner` queda visible en el campo de entrada | |

---

## Paso 2: Formular el Prompt Inicial con el Marco NECT

### Objetivo
Escribir un prompt descriptivo y completo que incluya Necesidad, Equipo, Contexto y Tiempo para que Planner Agent genere un plan de trabajo estructurado.

### Instrucciones

1. Con `@Planner` ya activado en el campo de texto, escribe el siguiente prompt. **Copia el texto completo** tal como aparece (puedes ajustar la fecha de inicio según la fecha actual de tu laboratorio):

   ```
   @Planner

   Soy el coordinador de operaciones de Distribuidora Andina S.A. y necesito 
   crear un plan de trabajo para preparar una auditoría interna de procesos 
   administrativos.

   CONTEXTO:
   - La auditoría interna está programada para dentro de 8 semanas a partir de hoy.
   - La empresa tiene 120 empleados distribuidos en 4 departamentos: Finanzas, 
     Logística, Recursos Humanos y Comercial.
   - Nunca hemos tenido una auditoría interna formal; es la primera vez.

   EQUIPO:
   - Marcela Ríos (líder del proyecto - coordinación general)
   - Jorge Castillo (analista financiero - revisión de procesos de Finanzas)
   - Patricia Vargas (especialista en RRHH - revisión de procesos de personal)
   - Daniel Morales (supervisor de logística - revisión de procesos operativos)

   ALCANCE:
   - Revisar y documentar los procesos administrativos clave de cada departamento.
   - Identificar brechas y riesgos en los controles internos.
   - Capacitar a los responsables de área sobre qué esperar en la auditoría.
   - Generar un informe de hallazgos y plan de remediación antes de la auditoría.

   TIEMPO:
   - Disponemos de exactamente 8 semanas.
   - La auditoría se realizará en la semana 9.

   Por favor, organiza el plan en 4 etapas: Preparación, Ejecución, Revisión 
   y Cierre. Cada etapa debe tener al menos 3 tareas con fechas de inicio y 
   fin, y asigna responsables del equipo a cada tarea.
   ```

2. Revisa el texto antes de enviarlo. Asegúrate de que no haya errores tipográficos que puedan confundir al agente.

3. Presiona **Enter** (o haz clic en el botón de enviar) para enviar el prompt.

4. Espera la respuesta de Planner Agent. Puede tomar entre 15 y 45 segundos generar el plan completo.

5. **Lee la respuesta completa** sin interactuar aún. Observa:
   - ¿El agente organizó el plan en las 4 etapas solicitadas?
   - ¿Cada etapa tiene al menos 3 tareas?
   - ¿Se asignaron fechas a las tareas?
   - ¿Se asignaron responsables del equipo?

### Resultado Esperado

Planner Agent responde con un plan estructurado que incluye aproximadamente:

- **Etapa 1 – Preparación** (Semanas 1-2): Tareas de diagnóstico, definición de alcance y comunicación inicial.
- **Etapa 2 – Ejecución** (Semanas 3-5): Tareas de levantamiento de procesos, revisión de controles y entrevistas.
- **Etapa 3 – Revisión** (Semanas 6-7): Tareas de análisis de hallazgos, elaboración de informe y validación.
- **Etapa 4 – Cierre** (Semana 8): Tareas de capacitación, ajustes finales y preparación logística.

Cada tarea incluye un responsable asignado del equipo de 4 personas y fechas tentativas.

> 📝 **NOTA**: La respuesta exacta puede variar. Lo importante es que contenga las 4 etapas, al menos 3 tareas por etapa, fechas y responsables. Si alguno de estos elementos falta, lo corregirás en el siguiente paso.

### Verificación

| Criterio | ✓ / ✗ |
|---|---|
| Planner Agent respondió sin errores | |
| El plan contiene exactamente 4 etapas (Preparación, Ejecución, Revisión, Cierre) | |
| Cada etapa tiene al menos 3 tareas | |
| Las tareas incluyen fechas de inicio y/o fin | |
| Los responsables ficticios están asignados a las tareas | |

---

## Paso 3: Refinar el Plan con Prompts de Seguimiento

### Objetivo
Usar comandos conversacionales de refinamiento para ajustar el plan: agregar tareas faltantes, modificar fechas y reorganizar responsabilidades.

### Instrucciones

1. **Refinamiento 1 — Agregar tarea de comunicación.** En el mismo hilo de conversación, escribe:

   ```
   Agrega una tarea en la Etapa 1 (Preparación) llamada "Comunicar el inicio 
   del proceso de auditoría a todos los líderes de departamento". Asígnala a 
   Marcela Ríos con fecha en la primera semana.
   ```

2. Espera la respuesta. Planner Agent debe confirmar la adición de la tarea y mostrar el plan actualizado (o al menos la etapa modificada).

3. **Refinamiento 2 — Ajustar fechas.** Escribe el siguiente prompt:

   ```
   Ajusta las fechas considerando que la auditoría interna se realizará 
   exactamente el lunes de la semana 9. Asegúrate de que la Etapa 4 (Cierre) 
   termine al menos 3 días hábiles antes de esa fecha para tener margen.
   ```

4. Espera la respuesta y verifica que las fechas de la Etapa 4 se hayan ajustado.

5. **Refinamiento 3 — Agregar tarea de contingencia.** Escribe:

   ```
   Agrega una tarea en la Etapa 3 (Revisión) llamada "Identificar y documentar 
   riesgos críticos que requieran remediación inmediata". Asígnala a Jorge 
   Castillo y Patricia Vargas como co-responsables.
   ```

6. Espera la confirmación del agente.

7. **Refinamiento 4 — Reorganizar prioridad.** Escribe:

   ```
   En la Etapa 2 (Ejecución), asegúrate de que la tarea de levantamiento 
   de procesos del departamento de Finanzas sea la primera en ejecutarse, 
   ya que es el área de mayor riesgo.
   ```

8. Revisa la respuesta final. El plan ahora debe reflejar todos los ajustes solicitados.

### Resultado Esperado

Después de los 4 refinamientos, el plan debe incluir:
- Una nueva tarea de comunicación en la Etapa 1 asignada a Marcela Ríos.
- Fechas ajustadas en la Etapa 4 que terminan al menos 3 días antes de la auditoría.
- Una tarea de riesgos críticos en la Etapa 3 con dos co-responsables.
- La tarea de Finanzas priorizada al inicio de la Etapa 2.

El plan total debe tener ahora **al menos 14 tareas** distribuidas en las 4 etapas.

### Verificación

| Criterio | ✓ / ✗ |
|---|---|
| La tarea de comunicación aparece en la Etapa 1 | |
| Las fechas de la Etapa 4 terminan antes de la semana de auditoría | |
| La tarea de riesgos críticos aparece en la Etapa 3 con dos responsables | |
| La tarea de Finanzas está priorizada en la Etapa 2 | |
| El plan mantiene coherencia general (sin duplicados ni contradicciones) | |

---

## Paso 4: Guardar el Plan en Microsoft Planner

### Objetivo
Confirmar la creación del plan en Microsoft Planner como un tablero funcional con el nombre especificado.

### Instrucciones

1. En el mismo hilo de conversación, escribe el siguiente prompt para solicitar la creación del plan:

   ```
   Crea este plan en Microsoft Planner con el nombre: 
   "Auditoría Interna - Distribuidora Andina"
   ```

2. Planner Agent mostrará un **resumen de confirmación** con el nombre del plan, número de tareas, fechas y un botón o enlace para confirmar la creación.

3. Haz clic en **"Confirmar"** (o "Create plan" / "Crear plan", según el idioma de tu interfaz).

4. Espera la confirmación del agente. Debe indicar que el plan fue creado exitosamente y proporcionarte un enlace para verlo en Planner.

5. Haz clic en el enlace proporcionado (o navega manualmente a `https://tasks.office.com`) para abrir Microsoft Planner.

6. En Microsoft Planner, localiza el plan **"Auditoría Interna - Distribuidora Andina"** en tu lista de planes.

7. Abre el plan y verifica que:
   - Las 4 etapas aparecen como **buckets** (cubetas/categorías) en la vista de tablero.
   - Las tareas están distribuidas correctamente en cada bucket.
   - Las fechas están asignadas (visibles al hacer clic en cada tarea).
   - Los responsables ficticios aparecen asignados (nota: si los nombres no coinciden con usuarios reales del tenant, pueden aparecer sin asignar — esto es normal en un entorno de práctica).

### Resultado Esperado

- El plan aparece en Microsoft Planner con el nombre exacto **"Auditoría Interna - Distribuidora Andina"**.
- La vista de tablero muestra 4 buckets correspondientes a las etapas: Preparación, Ejecución, Revisión y Cierre.
- Las tareas están organizadas dentro de sus respectivos buckets.
- Las fechas son visibles en las tarjetas de tarea o al abrirlas.

> 📝 **NOTA**: Si Planner Agent no ofrece la opción de crear el plan directamente (esto puede variar según la configuración del tenant), procede de la siguiente manera alternativa:
> - Abre Microsoft Planner manualmente (`https://tasks.office.com`).
> - Crea un nuevo plan con el nombre "Auditoría Interna - Distribuidora Andina".
> - Crea 4 buckets con los nombres de las etapas.
> - Agrega las tareas manualmente basándote en el plan que Planner Agent generó en la conversación.

### Verificación

| Criterio | ✓ / ✗ |
|---|---|
| El plan existe en Microsoft Planner con el nombre correcto | |
| Hay 4 buckets correspondientes a las 4 etapas | |
| Cada bucket contiene al menos 3 tareas | |
| Las tareas tienen fechas asignadas | |

---

## Paso 5: Exportar el Resumen del Plan a OneDrive

### Objetivo
Copiar el resumen textual del plan generado por Planner Agent y guardarlo como documento Word en OneDrive para uso en laboratorios posteriores.

### Instrucciones

1. Regresa a la conversación de **Copilot Chat** donde generaste el plan con Planner Agent.

2. Escribe el siguiente prompt para obtener un resumen limpio en formato texto:

   ```
   Genera un resumen ejecutivo del plan "Auditoría Interna - Distribuidora 
   Andina" en formato de texto plano, incluyendo: nombre del plan, objetivo, 
   equipo responsable, las 4 etapas con sus tareas, fechas y responsables. 
   Formatea con viñetas y encabezados claros.
   ```

3. Espera la respuesta. Planner Agent (o Copilot Chat) generará un resumen estructurado en texto.

4. **Selecciona todo el texto** de la respuesta del resumen (desde el título hasta la última tarea). Usa `Ctrl + A` dentro del bloque de respuesta o selecciona manualmente con el ratón.

5. **Copia el texto** con `Ctrl + C`.

6. Abre una nueva pestaña en el navegador y navega a tu **OneDrive**:
   ```
   https://onedrive.com
   ```

7. Navega a la carpeta **`Copilot_Labs`**.

8. Dentro de `Copilot_Labs`, crea un nuevo documento Word:
   - Haz clic en **"+ Nuevo"** (o "+ New").
   - Selecciona **"Documento de Word"** (o "Word document").
   - Se abrirá Word Online con un documento en blanco.

9. En el documento en blanco, **pega el contenido** con `Ctrl + V`.

10. Revisa que el contenido se haya pegado correctamente y que sea legible.

11. Haz clic en el **nombre del documento** en la parte superior (donde dice "Documento" o "Document") y renómbralo a:
    ```
    Plan_Auditoria_DistribuidoraAndina
    ```
    (Word Online agregará automáticamente la extensión `.docx`).

12. El documento se guarda automáticamente en OneDrive. Verifica que aparezca el indicador **"Guardado"** en la barra superior.

13. Cierra la pestaña de Word Online y regresa a OneDrive. Confirma que el archivo **`Plan_Auditoria_DistribuidoraAndina.docx`** aparece en la carpeta `Copilot_Labs`.

### Resultado Esperado

- El archivo **`Plan_Auditoria_DistribuidoraAndina.docx`** existe en `OneDrive > Copilot_Labs`.
- El contenido del archivo incluye:
  - Nombre del plan y objetivo.
  - Lista del equipo responsable (4 personas con roles).
  - Las 4 etapas con sus tareas, fechas y responsables.
- El archivo está guardado y accesible desde OneDrive.

### Verificación

| Criterio | ✓ / ✗ |
|---|---|
| El archivo `Plan_Auditoria_DistribuidoraAndina.docx` existe en `Copilot_Labs` | |
| El contenido incluye las 4 etapas del plan | |
| Cada etapa lista sus tareas con fechas y responsables | |
| El documento se guardó correctamente (indicador "Guardado" visible) | |

---

## Validación y Pruebas Finales

Antes de considerar el laboratorio completo, verifica los siguientes criterios de éxito:

### Lista de Validación Final

| # | Criterio de Éxito | Estado |
|---|---|---|
| 1 | Planner Agent fue identificado y activado correctamente en Copilot Chat | |
| 2 | El prompt inicial incluyó los 4 elementos del marco NECT (Necesidad, Equipo, Contexto, Tiempo) | |
| 3 | El plan generado contiene 4 etapas: Preparación, Ejecución, Revisión y Cierre | |
| 4 | Cada etapa tiene al menos 3 tareas específicas | |
| 5 | Se realizaron al menos 3 refinamientos conversacionales exitosos | |
| 6 | El plan existe en Microsoft Planner con el nombre "Auditoría Interna - Distribuidora Andina" | |
| 7 | El archivo `Plan_Auditoria_DistribuidoraAndina.docx` existe en `OneDrive > Copilot_Labs` | |
| 8 | El archivo Word contiene el resumen completo del plan con etapas, tareas, fechas y responsables | |

### Prueba de Integración

Para confirmar que el archivo será utilizable en el Laboratorio 04-03-01:

1. Abre el archivo `Plan_Auditoria_DistribuidoraAndina.docx` desde OneDrive.
2. Verifica que el contenido es legible y está bien estructurado.
3. Confirma que incluye suficiente contexto (nombre de empresa, objetivo de la auditoría, equipo, etapas completas) para que un lector sin contexto previo entienda el plan.

---

## Solución de Problemas

### Problema 1: Planner Agent no aparece en la lista de agentes

**Síntomas**: Al escribir `@` en Copilot Chat, la lista desplegable no muestra "Planner" como opción disponible. Solo aparecen otros agentes o ninguno.

**Causa**: La funcionalidad de Planner Agent puede no estar habilitada en el tenant, o la licencia de Microsoft 365 Copilot no incluye acceso a agentes especializados. También puede ocurrir si el administrador de IT ha restringido el acceso a agentes específicos.

**Solución**:
1. Verifica que tu licencia de Microsoft 365 Copilot está activa: navega a `https://myaccount.microsoft.com` y revisa tus suscripciones.
2. Intenta acceder desde **Microsoft Teams** en lugar de la interfaz web: abre Teams, ve al chat de Copilot y escribe `@Planner`.
3. Si el agente no está disponible en ninguna interfaz, notifica al instructor. Como alternativa, puedes completar el laboratorio usando **Copilot Chat general** (sin `@Planner`): escribe el mismo prompt sin el prefijo `@Planner`. Copilot generará el plan en texto (sin creación automática en Planner), y deberás crear el tablero manualmente en Microsoft Planner siguiendo la nota alternativa del Paso 4.

---

### Problema 2: El plan creado en Planner no muestra las fechas o los buckets correctamente

**Síntomas**: Al abrir el plan en Microsoft Planner, las tareas aparecen todas en un solo bucket (sin separación por etapas), o las fechas no están asignadas a las tarjetas de tarea.

**Causa**: Planner Agent puede generar la estructura de manera simplificada dependiendo de la complejidad de la solicitud o de limitaciones temporales en la integración. En algunos casos, el agente crea todas las tareas pero no las organiza en buckets separados.

**Solución**:
1. En Microsoft Planner, crea manualmente los 4 buckets si no existen:
   - Haz clic en **"+ Agregar bucket"** (o "+ Add bucket").
   - Nombra los buckets: `Preparación`, `Ejecución`, `Revisión`, `Cierre`.
2. Arrastra las tareas al bucket correspondiente según la etapa indicada en el plan textual de Copilot Chat.
3. Para agregar fechas faltantes: haz clic en cada tarea, selecciona **"Agregar fecha de inicio"** y **"Agregar fecha de vencimiento"**, y asigna las fechas según el plan generado.
4. Este ajuste manual toma aproximadamente 5-8 minutos y no afecta el cumplimiento del objetivo del laboratorio.

---

## Limpieza

Este laboratorio **no requiere limpieza** de recursos, ya que los artefactos generados serán utilizados en laboratorios posteriores:

- **Plan en Microsoft Planner** ("Auditoría Interna - Distribuidora Andina"): Mantener activo. No eliminar.
- **Archivo en OneDrive** (`Plan_Auditoria_DistribuidoraAndina.docx`): Mantener en la carpeta `Copilot_Labs`. Este archivo será insumo para el Laboratorio 04-03-01.
- **Conversación en Copilot Chat**: Se mantiene en el historial automáticamente. No es necesario guardarla por separado.

> ⚠️ **No elimines** el plan de Planner ni el archivo de Word. Ambos son necesarios para el siguiente laboratorio.

---

## Resumen

En este laboratorio aplicaste el flujo completo de transformación de una necesidad organizacional en un plan de trabajo estructurado usando Planner Agent:

| Fase del Laboratorio | Habilidad Desarrollada |
|---|---|
| Identificación del agente | Navegación en el ecosistema de agentes de Microsoft 365 Copilot |
| Formulación del prompt NECT | Redacción de prompts efectivos con contexto, equipo y restricciones |
| Refinamiento iterativo | Ajuste conversacional de planes mediante prompts de seguimiento |
| Guardado en Planner | Materialización de planes textuales en herramientas de gestión |
| Exportación a OneDrive | Creación de artefactos reutilizables para flujos encadenados |

### Conceptos Clave

- **Planner Agent** es un agente especializado dentro de Copilot Chat que conecta directamente con Microsoft Planner.
- El **marco NECT** (Necesidad, Equipo, Contexto, Tiempo) mejora significativamente la calidad de los planes generados.
- El **refinamiento iterativo** permite ajustar planes sin empezar de cero, manteniendo el contexto de la conversación.
- Los **flujos encadenados** (output de un laboratorio como input del siguiente) simulan ciclos reales de trabajo con IA corporativa.

### Recursos Adicionales

- [Documentación oficial de Microsoft Planner](https://support.microsoft.com/planner)
- [Guía de agentes de Microsoft 365 Copilot](https://learn.microsoft.com/microsoft-365-copilot/extensibility/)
- [Mejores prácticas para prompts en Copilot](https://adoption.microsoft.com/copilot/)

---

---

# Práctica guiada: Transformar información ficticia en una infografía ejecutiva con Copilot Chat

## Metadata

| Campo | Detalle |
|-------|---------|
| **Duración** | 50 minutos |
| **Complejidad** | Media |
| **Nivel Bloom** | Aplicar |
| **Dependencia** | Laboratorio 04-02-01 completado |
| **Entregables** | `Infografia_Auditoria_DistribuidoraAndina.png` (o `.html`) + sección "Resumen Ejecutivo Visual" en `Plan_Auditoria_DistribuidoraAndina.docx` |

---

## Descripción General

En este laboratorio transformarás la información del plan de auditoría generado en el Laboratorio 04-02-01 en una infografía ejecutiva destinada a la dirección general de Distribuidora Andina S.A. Aplicarás técnicas de identificación de información clave, definición de propósito y audiencia, y prompt engineering iterativo en Copilot Chat para producir un contenido visual estructurado que comunique los hallazgos más relevantes del plan de auditoría en un formato de alto impacto ejecutivo.

---

## Objetivos de Aprendizaje

Al finalizar este laboratorio, serás capaz de:

- [ ] Identificar y seleccionar los 5-7 indicadores, recomendaciones y resultados más relevantes del plan de auditoría para usarlos como base de la infografía
- [ ] Definir el propósito comunicacional (informar estado y obtener aprobación) y la audiencia objetivo (dirección general) de la infografía ejecutiva
- [ ] Formular prompts específicos en Copilot Chat que soliciten la generación de contenido infográfico estructurado a partir de información compleja
- [ ] Refinar iterativamente el contenido mediante al menos 3 ciclos de ajuste (estructura, métricas visuales y tono ejecutivo)
- [ ] Descargar la infografía generada y documentar el proceso completo de creación en el archivo Word del laboratorio anterior

---

## Prerrequisitos

### Conocimientos Previos

| Requisito | Descripción |
|-----------|-------------|
| Laboratorio 04-02-01 | Completado exitosamente; archivo `Plan_Auditoria_DistribuidoraAndina.docx` disponible |
| Infografía ejecutiva | Comprensión básica del concepto y su propósito (cubierto en módulo teórico 4.3) |
| Prompt engineering básico | Experiencia con formulación de prompts con contexto, objetivo y expectativas (Labs anteriores) |
| Patrones narrativos | Conocimiento de los patrones Situación→Hallazgo→Acción y Problema→Evidencia→Solución |

### Acceso y Recursos

| Recurso | Verificación |
|---------|-------------|
| Cuenta Microsoft 365 con licencia Copilot | Sesión activa en microsoft365.com |
| Copilot Chat | Acceso verificado en https://microsoft365.com/copilot con protección de datos comerciales activa |
| OneDrive | Carpeta `Copilot_Labs` visible con archivo `Plan_Auditoria_DistribuidoraAndina.docx` |
| Microsoft Planner | Tablero "Auditoría Interna - Distribuidora Andina" accesible como referencia |
| Microsoft Word Online | Acceso para edición del documento existente |

---

## Entorno del Laboratorio

### Hardware Mínimo

| Componente | Especificación |
|------------|---------------|
| Procesador | Intel Core i5 8ª gen. o AMD Ryzen 5 3000+ |
| RAM | 8 GB mínimo |
| Almacenamiento disponible | 2 GB libres |
| Internet | 10 Mbps descarga / 5 Mbps subida |
| Periféricos | Teclado, ratón/trackpad, pantalla con resolución mínima 1366×768 |

### Software Requerido

| Aplicación | Versión / Acceso |
|------------|-----------------|
| Microsoft Edge o Google Chrome | Edge 124+ o Chrome 124+ |
| Microsoft 365 Apps | Versión 2405 (Build 17628.20144) |
| Copilot Chat (web) | https://microsoft365.com/copilot |
| Microsoft Word Online | Acceso vía portal Microsoft 365 |
| OneDrive for Business | Cliente web o sincronización 24.071+ |

### Verificación Inicial del Entorno

Antes de comenzar, ejecuta estas verificaciones:

1. Navega a https://microsoft365.com/copilot e inicia sesión con tu cuenta corporativa
2. Confirma que aparece el mensaje: **"Tu organización tiene protección de datos comerciales activada"**
3. Abre OneDrive y navega a la carpeta `Copilot_Labs`
4. Verifica que el archivo `Plan_Auditoria_DistribuidoraAndina.docx` existe y puede abrirse
5. Abre el archivo y confirma que contiene el plan de auditoría completo del Lab 04-02-01

---

## Instrucciones Paso a Paso

### Paso 1: Revisar el plan de auditoría e identificar información clave

**Objetivo:** Extraer los 5-7 elementos más relevantes del plan de auditoría que servirán como contenido base de la infografía ejecutiva.

**Instrucciones:**

1. Abre el archivo `Plan_Auditoria_DistribuidoraAndina.docx` desde OneDrive > `Copilot_Labs` en Microsoft Word Online.

2. Lee el documento completo identificando mentalmente elementos que pertenezcan a estas tres categorías:
   - **Indicadores:** número de etapas, duración total, áreas auditadas, recursos asignados
   - **Resultados:** principales riesgos identificados, hallazgos esperados, estado del plan
   - **Recomendaciones:** acciones propuestas, prioridades, cronograma sugerido

3. Abre una nueva pestaña y navega a https://microsoft365.com/copilot

4. Copia el contenido completo del plan de auditoría y utiliza el siguiente prompt en Copilot Chat:

```
Actúa como un analista de auditoría interna. Tengo el siguiente plan de auditoría para Distribuidora Andina S.A.:

[PEGA AQUÍ EL CONTENIDO COMPLETO DEL PLAN DE AUDITORÍA]

Por favor, identifica y lista:
1. Los 5 indicadores cuantitativos más relevantes del plan (número de etapas, duración, áreas involucradas, recursos, etc.) con sus valores.
2. Los 3 principales resultados o hallazgos que se esperan de la auditoría.
3. Las recomendaciones de acción más importantes mencionadas en el plan.

Organiza la respuesta en tres secciones claramente separadas con viñetas.
Prioriza la información que sería más relevante para un comité directivo que necesita aprobar este plan.
```

5. Revisa la respuesta de Copilot y valida que los elementos identificados sean efectivamente los más relevantes. Si falta algún dato importante que recuerdes del documento, anótalo para incluirlo manualmente.

6. Copia la respuesta de Copilot y guárdala temporalmente en un bloc de notas o en un comentario dentro del documento Word para usarla en los pasos siguientes.

**Resultado Esperado:**

Una lista estructurada con aproximadamente 5-7 indicadores cuantitativos, 3 resultados principales y 2-4 recomendaciones de acción, todos extraídos del plan de auditoría. Ejemplo de elementos esperados:

- Número de etapas del plan: 4-5 fases
- Duración total estimada: X semanas/meses
- Áreas a auditar: finanzas, operaciones, cumplimiento, etc.
- Recursos requeridos: X auditores, X horas estimadas
- Principales riesgos: control interno, inventarios, etc.

**Verificación:**

- [ ] La lista contiene entre 5 y 7 indicadores cuantitativos con valores específicos
- [ ] Se identificaron al menos 3 resultados/hallazgos esperados
- [ ] Las recomendaciones están orientadas a la acción (verbos en infinitivo o imperativo)
- [ ] La información es verificable contra el documento original

---

### Paso 2: Definir propósito comunicacional y audiencia

**Objetivo:** Establecer explícitamente para quién es la infografía, qué decisión debe facilitar y qué patrón narrativo se utilizará.

**Instrucciones:**

1. En Copilot Chat, dentro de la misma conversación, ingresa el siguiente prompt para definir la estructura narrativa:

```
Ahora necesito transformar esta información en una infografía ejecutiva. Antes de generarla, ayúdame a definir la estructura:

AUDIENCIA: Dirección General de Distribuidora Andina S.A. (5 directores, perfil ejecutivo, máximo 2 minutos de atención)
PROPÓSITO: Informar sobre el plan de auditoría interna aprobado y comunicar alcance, cronograma y recursos necesarios para obtener respaldo ejecutivo.
PATRÓN NARRATIVO: Situación → Hallazgo → Acción

Con base en la información clave que identificaste anteriormente, propón:
1. Un título ejecutivo para la infografía (máximo 8 palabras)
2. La distribución de los elementos en las 3 secciones del patrón (Situación, Hallazgo, Acción)
3. Para cada elemento, indica: título corto (3-5 palabras), dato o mensaje clave, y tipo de visual sugerido (ícono, porcentaje, barra de progreso, semáforo, flecha de tendencia)

Limita el total a máximo 7 elementos principales.
```

2. Revisa la propuesta de estructura que genera Copilot. Evalúa:
   - ¿El título es claro y ejecutivo?
   - ¿La distribución entre secciones es equilibrada (no más de 3 elementos por sección)?
   - ¿Los tipos de visual sugeridos son apropiados para cada dato?

3. Si la estructura necesita ajustes, usa un prompt de refinamiento como:

```
Ajusta la estructura anterior:
- Cambia el título a algo que enfatice el impacto estratégico de la auditoría
- En la sección "Situación", incluye el contexto de por qué se necesita esta auditoría
- Asegúrate de que la sección "Acción" tenga al menos 2 elementos con fechas o plazos específicos
```

4. Una vez satisfecho con la estructura, cópiala y pégala como comentario o nota al final del documento Word para documentación.

**Resultado Esperado:**

Una estructura narrativa clara con:
- Título ejecutivo (ej: "Plan de Auditoría Interna 2024: Alcance y Ruta")
- Sección Situación: 2 elementos (contexto y justificación)
- Sección Hallazgo: 3 elementos (áreas clave, riesgos, recursos)
- Sección Acción: 2 elementos (cronograma, próximos pasos)
- Cada elemento con su tipo de visual asignado

**Verificación:**

- [ ] El título tiene máximo 8 palabras y comunica el tema central
- [ ] Los elementos están distribuidos en exactamente 3 secciones del patrón narrativo
- [ ] El total no excede 7 elementos principales
- [ ] Cada elemento tiene: título corto, dato clave y tipo de visual sugerido
- [ ] El contenido está orientado a la toma de decisiones ejecutivas (no a detalles operativos)

---

### Paso 3: Generar la infografía ejecutiva — Primer ciclo (estructura base)

**Objetivo:** Solicitar a Copilot Chat la generación del contenido visual estructurado de la infografía en su primera versión.

**Instrucciones:**

1. En la misma conversación de Copilot Chat, ingresa el siguiente prompt para generar la infografía:

```
Con base en la estructura que definimos, genera una infografía ejecutiva completa para la Dirección General de Distribuidora Andina S.A.

ESPECIFICACIONES DE FORMATO:
- Genera una imagen de infografía profesional con diseño vertical
- Estilo visual: corporativo, limpio, colores neutros (azul oscuro, gris, blanco con acentos en verde para elementos positivos y naranja para alertas)
- Tipografía: sans-serif, jerarquía clara entre títulos y datos
- Incluye el título ejecutivo en la parte superior
- Organiza las 3 secciones (Situación, Hallazgo, Acción) de arriba hacia abajo
- Usa íconos simples para cada elemento
- Los datos numéricos deben destacarse con tamaño de fuente mayor
- Incluye un pie de infografía con: "Distribuidora Andina S.A. | Auditoría Interna | [Mes Año]"

CONTENIDO A INCLUIR:
[Pega aquí la estructura de 7 elementos definida en el Paso 2]

Genera la infografía como imagen.
```

2. Observa la respuesta de Copilot. Dependiendo de las capacidades de tu tenant, Copilot puede:
   - **Opción A:** Generar una imagen directamente (usando DALL-E/Designer integrado)
   - **Opción B:** Generar código HTML/Markdown estructurado que representa la infografía
   - **Opción C:** Generar una descripción textual estructurada del contenido visual

3. **Si Copilot genera una imagen (Opción A):** Revisa la imagen generada sin descargarla aún. Identifica al menos 3 aspectos a mejorar (legibilidad de textos, jerarquía visual, datos faltantes, etc.). Anótalos para el siguiente ciclo de refinamiento.

4. **Si Copilot genera texto estructurado (Opciones B o C):** Esto es igualmente válido. El contenido estructurado es el insumo para la infografía. Continúa con el siguiente prompt alternativo:

```
Ahora genera una imagen de infografía basada en el contenido estructurado anterior. 
Crea una infografía visual profesional con:
- Fondo blanco o gris muy claro
- Secciones separadas por líneas o bloques de color
- Íconos representativos para cada elemento
- Números destacados en grande
- Diseño vertical, apto para impresión en A4
```

5. Registra en tu bloc de notas: el prompt exacto que usaste y una descripción breve del resultado obtenido (1-2 oraciones).

**Resultado Esperado:**

Una primera versión de la infografía (imagen o contenido estructurado) que contenga:
- Título ejecutivo visible en la parte superior
- Al menos 3 secciones diferenciadas visualmente
- Datos numéricos del plan de auditoría
- Elementos gráficos básicos (íconos, colores diferenciados, jerarquía tipográfica)
- Pie de infografía con identificación de la empresa

**Verificación:**

- [ ] Se obtuvo un output visual o estructurado (no solo texto plano sin formato)
- [ ] El título ejecutivo aparece de forma prominente
- [ ] Las 3 secciones del patrón narrativo son identificables
- [ ] Al menos 3 datos numéricos del plan de auditoría están presentes
- [ ] Se registró el prompt utilizado para documentación posterior

---

### Paso 4: Segundo ciclo de refinamiento — Métricas ficticias y formato visual

**Objetivo:** Mejorar la infografía incorporando métricas ficticias con formato visual impactante (porcentajes, semáforos de avance, indicadores de estado).

**Instrucciones:**

1. Analiza la primera versión generada e identifica oportunidades para agregar impacto visual mediante métricas. Luego ingresa el siguiente prompt de refinamiento:

```
Refina la infografía anterior con los siguientes ajustes de métricas y formato visual:

MÉTRICAS FICTICIAS A INCORPORAR:
- Cobertura de auditoría: 85% de procesos críticos (mostrar como barra de progreso circular)
- Estado de preparación: semáforo VERDE para documentación, AMARILLO para sistemas, VERDE para personal
- Inversión estimada: $45,000 USD (destacar con ícono de presupuesto)
- Duración del plan: 12 semanas (mostrar como línea de tiempo con 4 hitos)
- Riesgo residual esperado: reducción del 40% post-auditoría (mostrar como flecha descendente)

AJUSTES DE FORMATO:
- Los porcentajes deben aparecer en tamaño 2x más grande que el texto regular
- Usa un sistema de semáforo (verde/amarillo/rojo) para indicar estados
- Agrega flechas de tendencia (↑↓→) junto a las métricas comparativas
- Cada sección debe tener un borde o fondo de color diferente para distinguirlas claramente
- Los íconos deben ser minimalistas y profesionales

Genera la versión refinada como imagen.
```

2. Compara la nueva versión con la anterior. Verifica que:
   - Las métricas ficticias están incorporadas y son legibles
   - El sistema de semáforos o indicadores de estado es visible
   - La jerarquía visual mejoró (los datos importantes destacan más)

3. Si alguna métrica no se incorporó correctamente o el formato no es el deseado, realiza un ajuste puntual:

```
En la infografía anterior, ajusta lo siguiente:
- La barra de progreso del 85% debe ser más prominente y estar en la sección superior
- El semáforo de estados debe mostrarse como 3 círculos alineados horizontalmente con etiquetas debajo
- La línea de tiempo de 12 semanas debe mostrar los nombres de las 4 fases del plan
```

4. Registra en tu bloc de notas: el prompt de refinamiento y los cambios observados entre la versión 1 y la versión 2.

**Resultado Esperado:**

Una segunda versión de la infografía que incorpore:
- Al menos 4 métricas ficticias con formato visual diferenciado
- Sistema de semáforo o indicadores de estado con colores
- Porcentajes o cifras destacadas con tamaño mayor
- Flechas de tendencia o barras de progreso
- Mejor diferenciación visual entre secciones

**Verificación:**

- [ ] Al menos 4 de las 5 métricas ficticias solicitadas están presentes en la infografía
- [ ] Se observa un sistema de colores (verde/amarillo/rojo) para indicar estados
- [ ] Los números y porcentajes son visualmente prominentes (tamaño mayor o negrita)
- [ ] Existe una mejora observable respecto a la primera versión
- [ ] Se documentó el prompt de refinamiento utilizado

---

### Paso 5: Tercer ciclo de refinamiento — Tono ejecutivo y lenguaje final

**Objetivo:** Adaptar todo el texto de la infografía al nivel de lenguaje ejecutivo apropiado para la dirección general, eliminando jerga técnica y enfatizando el valor estratégico.

**Instrucciones:**

1. Revisa los textos visibles en la infografía actual. Identifica cualquier término técnico de auditoría que pueda no ser inmediatamente claro para un director general (ej: "control interno", "riesgo inherente", "materialidad", "hallazgo de no conformidad").

2. Ingresa el siguiente prompt de refinamiento de tono:

```
Realiza un tercer refinamiento de la infografía enfocado exclusivamente en el lenguaje y tono ejecutivo:

AJUSTES DE LENGUAJE:
- Reemplaza cualquier jerga técnica de auditoría por lenguaje de negocio
  Ejemplo: "Hallazgos de no conformidad" → "Oportunidades de mejora identificadas"
  Ejemplo: "Riesgo inherente" → "Exposición actual"
  Ejemplo: "Controles internos" → "Mecanismos de protección"
- Todos los títulos de sección deben ser orientados a acción o resultado (verbos o sustantivos de impacto)
  Ejemplo: "Fase de planificación" → "Ruta hacia la excelencia operativa"
- Las recomendaciones deben comenzar con verbos de acción ejecutiva: "Aprobar", "Priorizar", "Asignar", "Implementar"
- El tono general debe transmitir confianza y control, no alarma
- Agrega un subtítulo bajo el título principal que diga: "Resumen ejecutivo para aprobación de Dirección General"

AJUSTES FINALES DE PRESENTACIÓN:
- Verifica que ningún texto exceda 12 palabras por línea
- Los textos descriptivos no deben tener más de 2 líneas
- Agrega al pie: "Preparado por: Área de Auditoría Interna | Para: Comité de Dirección"

Genera la versión final como imagen.
```

3. Revisa la versión final generada. Lee cada texto visible y confirma que:
   - No hay jerga técnica sin traducir
   - El tono es profesional y orientado a decisiones
   - Los textos son concisos (máximo 2 líneas por elemento)
   - El subtítulo de audiencia está presente

4. Si necesitas un ajuste menor adicional, usa un prompt corto y específico:

```
En la versión final de la infografía, cambia únicamente:
- [Elemento específico a cambiar] por [nuevo texto deseado]
Mantén todo lo demás igual.
```

5. Registra el prompt de tono ejecutivo y los cambios observados en tu bloc de notas.

**Resultado Esperado:**

Versión final de la infografía con:
- Lenguaje 100% ejecutivo (sin jerga técnica de auditoría)
- Títulos orientados a acción o resultado
- Subtítulo que identifica la audiencia
- Textos concisos (ninguno mayor a 2 líneas)
- Pie de infografía con preparador y destinatario
- Tono que transmite confianza y control profesional

**Verificación:**

- [ ] No hay términos técnicos de auditoría sin traducir al lenguaje de negocio
- [ ] Todos los títulos de sección usan verbos de acción o sustantivos de impacto
- [ ] El subtítulo "Resumen ejecutivo para aprobación de Dirección General" está presente
- [ ] Ningún texto descriptivo excede 2 líneas
- [ ] El tono general es de confianza profesional, no de alarma o tecnicismo
- [ ] Se completaron los 3 ciclos de refinamiento documentados

---

### Paso 6: Descargar y guardar la infografía final

**Objetivo:** Guardar la infografía generada en el formato apropiado dentro de la estructura de carpetas del curso en OneDrive.

**Instrucciones:**

1. **Si Copilot generó una imagen:**
   - Haz clic derecho sobre la imagen generada en Copilot Chat
   - Selecciona "Guardar imagen como..." (o "Save image as...")
   - Navega a tu carpeta de OneDrive sincronizada: `OneDrive > Copilot_Labs`
   - Guarda el archivo con el nombre exacto: `Infografia_Auditoria_DistribuidoraAndina.png`

2. **Si Copilot generó contenido HTML/Markdown estructurado:**
   - Selecciona todo el contenido estructurado generado por Copilot
   - Abre un editor de texto (Bloc de notas o similar)
   - Pega el contenido y guárdalo como: `Infografia_Auditoria_DistribuidoraAndina.html`
   - Guarda el archivo en: `OneDrive > Copilot_Labs`

3. Verifica que el archivo se guardó correctamente:
   - Abre OneDrive en el navegador (onedrive.com)
   - Navega a la carpeta `Copilot_Labs`
   - Confirma que el archivo `Infografia_Auditoria_DistribuidoraAndina.png` (o `.html`) aparece en la lista
   - Haz clic en el archivo para verificar que se abre correctamente y muestra el contenido esperado

4. Si guardaste un archivo `.html`, ábrelo en el navegador para verificar que se renderiza correctamente y toma una captura de pantalla adicional como respaldo:
   - Presiona `Win + Shift + S` (Windows) o `Cmd + Shift + 4` (Mac)
   - Captura la infografía renderizada
   - Guarda la captura como `Infografia_Auditoria_DistribuidoraAndina_captura.png` en la misma carpeta

**Resultado Esperado:**

- Archivo `Infografia_Auditoria_DistribuidoraAndina.png` (o `.html`) guardado exitosamente en `OneDrive > Copilot_Labs`
- El archivo se abre correctamente y muestra la infografía completa con todos los elementos de los 3 ciclos de refinamiento

**Verificación:**

- [ ] El archivo existe en la ruta correcta: `OneDrive > Copilot_Labs > Infografia_Auditoria_DistribuidoraAndina.png` (o `.html`)
- [ ] El archivo se abre sin errores y muestra contenido visual
- [ ] El nombre del archivo es exactamente el especificado (sin espacios adicionales ni caracteres especiales)
- [ ] El archivo tiene un tamaño razonable (>50 KB para imagen, >2 KB para HTML)

---

### Paso 7: Documentar el proceso en el archivo Word

**Objetivo:** Actualizar el archivo `Plan_Auditoria_DistribuidoraAndina.docx` con una nueva sección que documente todo el proceso de creación de la infografía.

**Instrucciones:**

1. Abre el archivo `Plan_Auditoria_DistribuidoraAndina.docx` en Word Online desde OneDrive > `Copilot_Labs`.

2. Desplázate al final del documento y agrega un salto de página (Insertar > Salto de página).

3. Crea una nueva sección con el título de nivel 1: **"Resumen Ejecutivo Visual"**

4. Estructura la sección con los siguientes subtítulos y contenido:

```
## Resumen Ejecutivo Visual

### Propósito de la Infografía
[Describe en 2-3 oraciones el objetivo comunicacional: informar a la Dirección General 
sobre el plan de auditoría para obtener aprobación y respaldo ejecutivo]

### Audiencia Objetivo
- Destinatario: Dirección General de Distribuidora Andina S.A.
- Perfil: Ejecutivos de alto nivel, tiempo limitado de atención
- Decisión esperada: Aprobación del plan y asignación de recursos

### Patrón Narrativo Utilizado
Situación → Hallazgo → Acción

### Información Clave Seleccionada
[Lista con viñetas de los 5-7 elementos que se incluyeron en la infografía]

### Proceso de Refinamiento Iterativo

#### Ciclo 1 — Estructura Base
- Prompt utilizado: [Pega el prompt del Paso 3]
- Resultado: [Descripción breve de lo obtenido]
- Aspectos a mejorar identificados: [Lista]

#### Ciclo 2 — Métricas y Formato Visual
- Prompt utilizado: [Pega el prompt del Paso 4]
- Cambios observados: [Descripción de mejoras]
- Métricas incorporadas: [Lista]

#### Ciclo 3 — Tono Ejecutivo
- Prompt utilizado: [Pega el prompt del Paso 5]
- Ajustes de lenguaje realizados: [Ejemplos de antes/después]
- Resultado final: [Evaluación breve]

### Archivo de Infografía
- Nombre: Infografia_Auditoria_DistribuidoraAndina.png [o .html]
- Ubicación: OneDrive > Copilot_Labs
- Fecha de generación: [Fecha actual]

### Lecciones Aprendidas
[2-3 observaciones sobre qué funcionó bien y qué mejorarías en futuros ejercicios 
de generación de infografías con Copilot Chat]
```

5. Completa cada sección con la información real de tu proceso (prompts exactos, descripciones de resultados, observaciones).

6. Si es posible, inserta la imagen de la infografía dentro del documento Word:
   - Posiciona el cursor después del título "Resumen Ejecutivo Visual"
   - Ve a Insertar > Imagen > Desde este dispositivo (o desde OneDrive)
   - Selecciona `Infografia_Auditoria_DistribuidoraAndina.png`
   - Ajusta el tamaño para que ocupe el ancho de la página

7. Guarda el documento (Ctrl+S o se guarda automáticamente en Word Online).

**Resultado Esperado:**

El archivo `Plan_Auditoria_DistribuidoraAndina.docx` ahora contiene:
- Todo el contenido original del plan de auditoría (Lab 04-02-01)
- Una nueva sección "Resumen Ejecutivo Visual" al final
- Documentación completa de los 3 ciclos de refinamiento con prompts exactos
- La imagen de la infografía insertada (si fue posible técnicamente)
- Sección de lecciones aprendidas

**Verificación:**

- [ ] La sección "Resumen Ejecutivo Visual" existe como última sección del documento
- [ ] Se documentaron los 3 prompts de refinamiento (uno por ciclo)
- [ ] Cada ciclo incluye: prompt usado, resultado obtenido y cambios observados
- [ ] La sección "Lecciones Aprendidas" contiene al menos 2 observaciones
- [ ] El documento se guardó exitosamente sin errores

---

## Validación y Pruebas Finales

Antes de considerar el laboratorio completado, verifica los siguientes criterios de éxito:

### Lista de Verificación de Entregables

| # | Entregable | Criterio de Aceptación | ✓ |
|---|-----------|----------------------|---|
| 1 | Información clave identificada | 5-7 elementos extraídos del plan de auditoría | ☐ |
| 2 | Estructura narrativa definida | Patrón Situación→Hallazgo→Acción con máx. 7 elementos | ☐ |
| 3 | Infografía V1 generada | Primera versión con estructura base visible | ☐ |
| 4 | Infografía V2 con métricas | Métricas ficticias y formato visual incorporados | ☐ |
| 5 | Infografía V3 final | Tono ejecutivo, sin jerga técnica, textos concisos | ☐ |
| 6 | Archivo de infografía guardado | `Infografia_Auditoria_DistribuidoraAndina.png/.html` en `Copilot_Labs` | ☐ |
| 7 | Documentación en Word | Sección "Resumen Ejecutivo Visual" completa con 3 ciclos documentados | ☐ |

### Validación de Calidad del Contenido

Aplica estos criterios a tu infografía final:

- **Claridad:** ¿Un ejecutivo sin contexto previo podría entender el mensaje principal en menos de 30 segundos?
- **Completitud:** ¿Los 5-7 elementos clave del plan de auditoría están representados?
- **Jerarquía:** ¿Se distingue claramente qué información es más importante?
- **Accionabilidad:** ¿La sección de "Acción" deja claro qué se espera de la dirección?
- **Profesionalismo:** ¿El tono y la estética son apropiados para un comité directivo?

---

## Solución de Problemas

### Problema 1: Copilot Chat no genera imágenes, solo texto

**Síntomas:** Al solicitar "genera una infografía como imagen", Copilot responde con texto estructurado, listas o código Markdown pero no produce una imagen visual. Puede mostrar un mensaje como "No puedo generar imágenes en este momento" o simplemente omitir la generación visual.

**Causa:** El tenant de Microsoft 365 puede no tener habilitada la capacidad de generación de imágenes (DALL-E/Designer) dentro de Copilot Chat, o la licencia asignada no incluye esta funcionalidad. Esto varía según la configuración del administrador y la versión del servicio.

**Solución:**

1. No consideres esto un error bloqueante. El laboratorio está diseñado para funcionar con ambas modalidades.
2. Trabaja con el contenido estructurado (texto/HTML/Markdown) que Copilot sí genera.
3. Modifica tu prompt para solicitar explícitamente un formato alternativo:

```
Ya que no puedes generar una imagen directamente, genera el contenido de la infografía 
en formato HTML con estilos CSS inline que pueda renderizarse en un navegador web.
Incluye colores, tamaños de fuente diferenciados, bordes y espaciado que simulen 
una infografía profesional.
```

4. Guarda el output como archivo `.html` en lugar de `.png`.
5. Abre el archivo HTML en tu navegador y toma una captura de pantalla para obtener la versión `.png`.
6. Documenta en la sección de "Lecciones Aprendidas" que tu tenant no tenía habilitada la generación de imágenes y cómo resolviste la situación.

---

### Problema 2: El contenido de la infografía no refleja los datos del plan de auditoría

**Síntomas:** Copilot genera una infografía genérica sobre auditoría que no incluye los datos específicos de Distribuidora Andina S.A. (nombres de áreas, cifras del plan, cronograma específico). Los datos parecen inventados por Copilot en lugar de provenir del documento original.

**Causa:** El prompt no incluyó suficiente contexto específico del plan de auditoría, o el contenido pegado se truncó por exceder el límite de caracteres de la ventana de chat. Copilot "rellenó" con información genérica al no tener los datos específicos disponibles.

**Solución:**

1. Verifica que el contenido del plan de auditoría se pegó completamente en el primer prompt del Paso 1. Si el documento es muy extenso, divídelo en secciones.
2. En lugar de pegar todo el documento, usa la lista de información clave ya extraída (resultado del Paso 1) como input directo:

```
Usa EXCLUSIVAMENTE los siguientes datos para la infografía. No inventes ni agregues 
información que no esté en esta lista:

[Pega aquí la lista exacta de los 5-7 elementos identificados en el Paso 1, 
con sus valores específicos]

Empresa: Distribuidora Andina S.A.
Contexto: Plan de auditoría interna [año]
[Incluye 2-3 datos específicos adicionales del plan original]
```

3. Al revisar cada versión, verifica activamente que los datos mostrados coincidan con tu documento original. Si detectas datos inventados, señálalos específicamente:

```
En la infografía anterior, corrige lo siguiente:
- Donde dice "[dato incorrecto]" debe decir "[dato correcto del plan]"
- El número de áreas auditadas es [X], no [Y]
- La duración correcta es [Z semanas], no [W meses]
```

4. Mantén el documento Word abierto en otra pestaña para poder hacer verificaciones cruzadas rápidas.

---

## Limpieza del Entorno

Al finalizar el laboratorio, asegúrate de:

1. **Guardar todos los archivos:** Confirma que tanto `Infografia_Auditoria_DistribuidoraAndina.png` (o `.html`) como `Plan_Auditoria_DistribuidoraAndina.docx` (actualizado) están sincronizados en OneDrive > `Copilot_Labs`.

2. **No cerrar la conversación de Copilot Chat** si tu tenant permite guardar el historial. Esta conversación podrá ser referenciada en el Laboratorio 04-04-01.

3. **Verificar la estructura de carpetas:**
   ```
   OneDrive/
   └── Copilot_Labs/
       ├── Plan_Auditoria_DistribuidoraAndina.docx  (actualizado con sección visual)
       ├── Infografia_Auditoria_DistribuidoraAndina.png  (o .html)
       └── [otros archivos de laboratorios anteriores]
   ```

4. **No eliminar** ningún archivo de laboratorios anteriores, ya que el Lab 04-04-01 requiere tanto el plan como la infografía como insumos.

---

## Resumen

En este laboratorio aplicaste el flujo completo de transformación de información compleja en una infografía ejecutiva utilizando Copilot Chat:

| Fase | Actividad Realizada | Habilidad Desarrollada |
|------|--------------------|-----------------------|
| Identificación | Extrajiste 5-7 elementos clave del plan de auditoría | Destilación de información con filtros de relevancia |
| Definición | Estableciste audiencia, propósito y patrón narrativo | Pensamiento estratégico de comunicación |
| Generación | Creaste la primera versión de la infografía | Prompt engineering para contenido visual |
| Refinamiento 1 | Incorporaste métricas ficticias con formato visual | Iteración con especificaciones cuantitativas |
| Refinamiento 2 | Adaptaste el tono al nivel ejecutivo | Ajuste de lenguaje para audiencias específicas |
| Documentación | Registraste el proceso completo en Word | Trazabilidad y reproducibilidad del trabajo con IA |

**Conceptos clave reforzados:**
- La infografía ejecutiva no reemplaza el reporte; lo complementa para abrir la conversación
- El refinamiento iterativo (mínimo 3 ciclos) produce resultados significativamente mejores que un solo prompt
- Definir audiencia y propósito ANTES de generar contenido es crítico para la calidad del output
- La documentación del proceso permite reproducir y mejorar el flujo de trabajo en futuras ocasiones

**Conexión con el siguiente laboratorio:** El archivo `Plan_Auditoria_DistribuidoraAndina.docx` actualizado y la infografía `Infografia_Auditoria_DistribuidoraAndina.png` serán utilizados como contexto de Distribuidora Andina S.A. en el Laboratorio 04-04-01.

### Recursos Adicionales

- Módulo teórico 4.3: "De información compleja a una infografía ejecutiva" — para revisión de patrones narrativos
- Microsoft Learn: [Copilot Chat best practices](https://learn.microsoft.com/copilot/microsoft-365) — documentación oficial sobre capacidades de generación
- Referencia de patrones narrativos: Situación→Hallazgo→Acción | Problema→Evidencia→Solución | Antes→Durante→Después

---

# Práctica guiada: Analizar comentarios de clientes con Copilot Chat, generar gráficos y proponer acciones de mejora

## Metadata

| Campo | Detalle |
|-------|---------|
| **Duración** | 40 minutos |
| **Complejidad** | Media |
| **Nivel Bloom** | Analizar |
| **Módulo** | 4.4 — Análisis de comentarios para identificar oportunidades de mejora |
| **Batch** | 2 (Laboratorio final — integra outputs de Labs 04-02-01 y 04-03-01) |

---

## Descripción general

En este laboratorio asumirás el rol de analista de experiencia del cliente en **Distribuidora Andina S.A.** Como parte del proceso de auditoría interna planificado en el Laboratorio 04-02-01, se recopilaron 30 comentarios ficticios de clientes sobre el servicio de distribución. Utilizarás Copilot Chat para realizar un análisis cualitativo completo: identificar temas recurrentes, generar gráficos visuales descargables, priorizar hallazgos críticos y proponer acciones de mejora concretas. Finalmente, consolidarás todos los outputs del batch en un reporte ejecutivo integrado.

---

## Objetivos de aprendizaje

Al completar este laboratorio serás capaz de:

- [ ] Preparar y estructurar un conjunto de 30 comentarios ficticios en un archivo Word optimizado para análisis con IA
- [ ] Formular prompts progresivos que identifiquen temas recurrentes, sentimientos predominantes y áreas de mejora
- [ ] Generar al menos 2 gráficos visuales descargables (frecuencia de temas y distribución de sentimientos) mediante Copilot Chat
- [ ] Refinar solicitudes para priorizar hallazgos críticos y obtener propuestas de acciones de mejora accionables
- [ ] Integrar los resultados del análisis en un documento consolidado que demuestre el uso encadenado de Copilot Chat a lo largo del batch

---

## Prerrequisitos

### Conocimientos previos

| Requisito | Descripción |
|-----------|-------------|
| Laboratorio 04-02-01 completado | Archivo `Plan_Auditoria_DistribuidoraAndina.docx` disponible en `Copilot_Labs` |
| Laboratorio 04-03-01 completado | Archivo `Infografia_Auditoria_DistribuidoraAndina.png` (o equivalente) disponible en `Copilot_Labs` |
| Análisis cualitativo básico | Comprensión de categorización temática y análisis de sentimiento (cubierto en módulo teórico 4.4) |
| Prompt engineering | Dominio de la estructura contexto-objetivo-fuentes-expectativas para formular prompts |

### Acceso y licencias

| Recurso | Verificación requerida |
|---------|----------------------|
| Cuenta Microsoft 365 corporativa | Sesión activa en `microsoft365.com` con cuenta `@contoso-curso.onmicrosoft.com` |
| Licencia Microsoft 365 Copilot | Verificar mensaje "Tu organización tiene protección de datos comerciales activada" en `microsoft365.com/copilot` |
| OneDrive for Business | Carpeta `Copilot_Labs` existente con archivos de labs anteriores |
| Microsoft Word Online | Acceso funcional desde el portal Microsoft 365 |

---

## Entorno del laboratorio

### Software requerido

| Aplicación | Versión / Acceso |
|------------|-----------------|
| Microsoft Copilot Chat (web) | `microsoft365.com/copilot` — con protección de datos comerciales |
| Microsoft Word Online | Build 2405 (acceso vía portal Microsoft 365) |
| Microsoft OneDrive (web) | Versión sincronización 24.071.0407.0003 |
| Microsoft Edge o Google Chrome | Edge 124+ o Chrome 124+ |

### Estructura de archivos esperada al inicio

```
OneDrive/
└── Copilot_Labs/
    ├── Plan_Auditoria_DistribuidoraAndina.docx    ← del Lab 04-02-01
    └── Infografia_Auditoria_DistribuidoraAndina.png  ← del Lab 04-03-01
```

### Estructura de archivos esperada al finalizar

```
OneDrive/
└── Copilot_Labs/
    ├── Plan_Auditoria_DistribuidoraAndina.docx
    ├── Infografia_Auditoria_DistribuidoraAndina.png
    ├── Comentarios_Clientes_DistribuidoraAndina.docx  ← NUEVO
    ├── Grafico_Temas_Clientes.png                      ← NUEVO
    ├── Grafico_Sentimientos_Clientes.png               ← NUEVO
    └── Reporte_Final_Auditoria_DistribuidoraAndina.docx ← NUEVO
```

---

## Instrucciones paso a paso

### Paso 1: Crear el archivo de comentarios de clientes

**Objetivo:** Preparar un documento Word estructurado con los 30 comentarios ficticios que servirá como insumo para el análisis con Copilot Chat.

**Instrucciones:**

1. Abre tu navegador y navega a `https://microsoft365.com`.
2. Inicia sesión con tu cuenta corporativa `@contoso-curso.onmicrosoft.com`.
3. En el panel lateral izquierdo, haz clic en **OneDrive**.
4. Navega a la carpeta `Copilot_Labs`.
5. Haz clic en **+ Nuevo** → **Documento de Word**.
6. Renombra el archivo como `Comentarios_Clientes_DistribuidoraAndina.docx`.
7. En la primera línea del documento, escribe el siguiente encabezado:

```
Dataset: Distribuidora Andina S.A. - Comentarios de clientes sobre servicio de distribución
Período: Q1 2025
Total de registros: 30
Categorías cubiertas: Tiempos de entrega, Calidad del producto, Atención al cliente, Facturación, Comunicación postventa
```

8. Deja una línea en blanco y copia los siguientes 30 comentarios exactamente como aparecen:

```
01. "El pedido llegó 5 días después de la fecha prometida. Inaceptable para productos perecederos."
02. "La calidad del producto es excelente, siempre llega en perfectas condiciones."
03. "Llamé tres veces al servicio al cliente y nadie pudo darme el número de seguimiento."
04. "Me facturaron dos veces el mismo despacho. Tardaron 3 semanas en hacer la nota de crédito."
05. "Nunca recibí confirmación de que mi pedido fue despachado. Me enteré cuando llegó."
06. "Los tiempos de entrega han mejorado mucho en los últimos dos meses. Felicitaciones."
07. "El producto llegó con el empaque dañado y dos unidades rotas."
08. "La ejecutiva de cuentas fue muy atenta y resolvió mi reclamo en menos de 24 horas."
09. "Llevo esperando una factura corregida desde hace un mes. Nadie me responde."
10. "No hay forma de rastrear el pedido en línea. Necesitan una plataforma de seguimiento."
11. "Excelente relación calidad-precio. Los productos siempre cumplen especificaciones."
12. "El camión llegó fuera del horario acordado y no había personal para recibir."
13. "El área de facturación no contesta el teléfono. Solo responden por correo y tardan días."
14. "Después de cada entrega recibo una encuesta de satisfacción. Eso demuestra que les importa."
15. "Pedí un cambio de dirección de entrega con 48 horas de anticipación y no lo registraron."
16. "La calidad de los productos frescos ha bajado notablemente este trimestre."
17. "El agente de atención al cliente fue grosero cuando pregunté por mi reembolso."
18. "Me cobraron un recargo por entrega urgente que nunca solicité."
19. "Nunca me avisaron que el producto estaba en backorder. Me enteré al reclamar."
20. "Entrega puntual, producto en buen estado. Sin quejas."
21. "El sistema de facturación genera errores cuando hay descuentos por volumen."
22. "Tres entregas consecutivas con retraso de más de 48 horas."
23. "El equipo de postventa me contactó para verificar que todo estuviera bien. Muy profesional."
24. "La calidad del empaque ha mejorado. Ya no llegan productos dañados."
25. "Imposible comunicarse con el área de despacho. No hay un canal directo."
26. "Me enviaron el producto equivocado y tardaron una semana en recogerlo."
27. "La factura electrónica siempre llega a tiempo y sin errores. Buen sistema."
28. "No existe comunicación proactiva. Solo me entero de retrasos cuando llamo yo."
29. "El precio es competitivo y la entrega generalmente cumple los plazos."
30. "Solicité una cotización hace dos semanas y nadie me ha respondido."
```

9. Guarda el documento (se guarda automáticamente en Word Online, pero verifica que aparezca "Guardado" en la barra superior).

**Output esperado:** Documento Word con encabezado descriptivo y 30 comentarios numerados, guardado en `Copilot_Labs`.

**Verificación:**
- [ ] El archivo aparece en `OneDrive > Copilot_Labs` con el nombre correcto
- [ ] Los 30 comentarios están numerados del 01 al 30
- [ ] El encabezado incluye el nombre de la empresa, período y categorías

---

### Paso 2: Cargar los comentarios en Copilot Chat e identificar temas recurrentes (Fase 1)

**Objetivo:** Formular un prompt de análisis cualitativo que permita a Copilot Chat identificar los temas principales, su frecuencia y el sentimiento asociado.

**Instrucciones:**

1. Abre una nueva pestaña del navegador y navega a `https://microsoft365.com/copilot`.
2. Verifica que en la parte inferior de la interfaz aparezca el mensaje **"Tu organización tiene protección de datos comerciales activada"**. Si no aparece, detente y notifica al instructor.
3. En la interfaz de Copilot Chat, haz clic en el ícono de **adjuntar archivo** (ícono de clip o "+") ubicado junto al cuadro de texto.
4. Selecciona **OneDrive** como origen y navega a `Copilot_Labs`.
5. Selecciona el archivo `Comentarios_Clientes_DistribuidoraAndina.docx` y confirma la carga.

> **Nota alternativa:** Si tu tenant no permite adjuntar archivos directamente, selecciona todo el contenido del documento Word (Ctrl+A), cópialo (Ctrl+C) y pégalo (Ctrl+V) directamente en el cuadro de mensaje de Copilot Chat antes del prompt.

6. Escribe el siguiente prompt en el cuadro de mensaje y presiona Enter:

```
Contexto: Soy analista de experiencia del cliente en Distribuidora Andina S.A., 
una empresa de distribución de productos con 500 empleados. Estamos realizando 
una auditoría interna del servicio al cliente.

Tarea: Analiza los 30 comentarios de clientes que te comparto en el archivo adjunto 
y realiza lo siguiente:

1. Identifica los temas principales que mencionan los clientes.
2. Agrúpalos en exactamente 5 categorías temáticas: Tiempos de entrega, 
   Calidad del producto, Atención al cliente, Facturación, y Comunicación postventa.
3. Indica cuántos comentarios pertenecen a cada categoría (un comentario puede 
   pertenecer a una sola categoría principal).
4. Para cada categoría, clasifica el sentimiento predominante como: Positivo, 
   Negativo o Mixto.
5. Lista los números de comentario que pertenecen a cada categoría.

Formato de salida: Presenta los resultados en una tabla ordenada de mayor a menor 
frecuencia. Incluye una columna adicional con los números de comentario asignados.
```

7. Espera la respuesta de Copilot Chat. Revisa la tabla generada.
8. Copia la respuesta completa de Copilot (selecciona el texto de la respuesta y usa Ctrl+C) y guárdala temporalmente en un bloc de notas o en un documento aparte para uso posterior.

**Output esperado:** Una tabla similar a esta (los números exactos pueden variar ligeramente):

| Categoría | N.º de comentarios | Sentimiento | Comentarios asignados |
|-----------|-------------------|-------------|----------------------|
| Tiempos de entrega | 8 | Negativo | 01, 06, 12, 15, 20, 22, 26, 29 |
| Facturación | 7 | Negativo | 04, 09, 13, 18, 21, 27, 07* |
| Comunicación postventa | 6 | Negativo | 05, 10, 19, 25, 28, 30 |
| Atención al cliente | 5 | Mixto | 03, 08, 14, 17, 23 |
| Calidad del producto | 4 | Mixto | 02, 11, 16, 24 |

> *Nota: La asignación exacta puede variar según la interpretación de Copilot. Lo importante es que las 5 categorías estén presentes y la distribución sea razonable.*

**Verificación:**
- [ ] Copilot Chat generó una tabla con exactamente 5 categorías
- [ ] Cada categoría tiene un conteo de comentarios y un sentimiento asignado
- [ ] La suma total de comentarios asignados se aproxima a 30
- [ ] El sentimiento predominante general es negativo/mixto (consistente con la distribución 60-40 del dataset)

---

### Paso 3: Generar gráfico de frecuencia de temas (Fase 2)

**Objetivo:** Solicitar a Copilot Chat la generación de un gráfico de barras que muestre la frecuencia de cada categoría temática, descargarlo como imagen.

**Instrucciones:**

1. En la misma conversación de Copilot Chat (no abras una nueva), escribe el siguiente prompt:

```
Basándote en la tabla de análisis que acabas de generar, crea un gráfico de barras 
horizontales que muestre las 5 categorías temáticas en el eje Y y el número de 
comentarios en el eje X. 

Especificaciones del gráfico:
- Título: "Distribuidora Andina S.A. - Temas más frecuentes en comentarios de clientes (Q1 2025)"
- Las barras deben estar ordenadas de mayor a menor frecuencia (la categoría con más comentarios arriba)
- Usa colores diferenciados para cada barra
- Incluye el valor numérico al final de cada barra
- Estilo profesional y limpio, apto para un reporte ejecutivo

Genera el gráfico como una imagen que pueda descargar.
```

2. Espera a que Copilot Chat genere la imagen del gráfico.
3. Cuando aparezca el gráfico en la respuesta, haz clic derecho sobre la imagen.
4. Selecciona **"Guardar imagen como..."** (o la opción equivalente en tu navegador).
5. Navega a `OneDrive > Copilot_Labs` en el diálogo de guardado.
6. Guarda el archivo con el nombre exacto: `Grafico_Temas_Clientes.png`.

> **Alternativa si Copilot no genera la imagen directamente:** Si Copilot Chat responde con una descripción del gráfico o código en lugar de una imagen, reformula el prompt así: "Genera una imagen visual de este gráfico de barras. Necesito descargarla como archivo PNG." Si persiste el problema, Copilot puede ofrecer un botón de descarga debajo de la imagen generada — haz clic en él.

7. Verifica que el archivo se guardó correctamente abriendo OneDrive en otra pestaña.

**Output esperado:** Imagen PNG de un gráfico de barras horizontales con 5 barras representando las categorías temáticas, ordenadas de mayor a menor frecuencia, con título profesional y valores numéricos visibles.

**Verificación:**
- [ ] La imagen del gráfico se descargó exitosamente
- [ ] El archivo `Grafico_Temas_Clientes.png` existe en la carpeta `Copilot_Labs`
- [ ] El gráfico muestra las 5 categorías con valores numéricos
- [ ] El título del gráfico incluye el nombre de la empresa y el período

---

### Paso 4: Generar gráfico de distribución de sentimientos (Fase 3)

**Objetivo:** Solicitar un segundo gráfico que visualice la proporción de sentimientos (positivo, negativo, mixto) en el conjunto total de comentarios.

**Instrucciones:**

1. Continuando en la misma conversación de Copilot Chat, escribe el siguiente prompt:

```
Ahora necesito un segundo gráfico. Basándote en el análisis de los 30 comentarios, 
clasifica CADA comentario individual según su sentimiento: Positivo, Negativo o Neutral.

Luego genera un gráfico circular (pie chart) que muestre la distribución porcentual 
de sentimientos en el total de los 30 comentarios.

Especificaciones:
- Título: "Distribución de sentimientos - Comentarios de clientes Q1 2025"
- Muestra el porcentaje y el número absoluto de comentarios para cada segmento
- Usa los colores: verde para Positivo, rojo para Negativo, amarillo/gris para Neutral
- Estilo profesional, limpio y ejecutivo
- Genera la imagen para descarga

Antes de generar el gráfico, muéstrame la clasificación de cada comentario 
en una tabla breve para que pueda validar la distribución.
```

2. Revisa la tabla de clasificación individual que Copilot Chat genere. Valida que la distribución sea aproximadamente:
   - **Negativo:** 16-18 comentarios (~55-60%)
   - **Positivo:** 9-11 comentarios (~30-35%)
   - **Neutral:** 2-4 comentarios (~7-13%)

3. Si la distribución te parece razonable, confirma a Copilot: "La clasificación se ve bien. Genera el gráfico circular ahora."

4. Cuando aparezca la imagen del gráfico circular, descárgala con clic derecho → **"Guardar imagen como..."**

5. Guarda el archivo en `OneDrive > Copilot_Labs` con el nombre: `Grafico_Sentimientos_Clientes.png`.

**Output esperado:** Imagen PNG de un gráfico circular (pie chart) con tres segmentos coloreados que muestran la distribución de sentimientos, con porcentajes y valores absolutos visibles.

**Verificación:**
- [ ] Copilot Chat proporcionó una tabla de clasificación individual antes del gráfico
- [ ] La distribución muestra mayoría de sentimiento negativo (~60%), consistente con el diseño del dataset
- [ ] El archivo `Grafico_Sentimientos_Clientes.png` se guardó en `Copilot_Labs`
- [ ] El gráfico incluye título, porcentajes y leyenda de colores

---

### Paso 5: Refinar el análisis para priorización y propuesta de acciones (Fase 4)

**Objetivo:** Solicitar a Copilot Chat que priorice los 3 hallazgos más críticos y proponga acciones de mejora concretas para cada uno, generando una síntesis ejecutiva.

**Instrucciones:**

1. En la misma conversación, escribe el siguiente prompt de refinamiento:

```
Excelente análisis. Ahora necesito una síntesis ejecutiva para presentar 
al Comité de Dirección de Distribuidora Andina S.A.

Basándote en todo el análisis que hemos realizado, haz lo siguiente:

1. PRIORIZACIÓN: Identifica los 3 hallazgos más críticos que representan 
   mayor riesgo para la retención de clientes. Ordénalos por nivel de 
   urgencia (Alta, Media-Alta, Media). Justifica cada priorización con 
   evidencia específica de los comentarios.

2. ACCIONES DE MEJORA: Para cada hallazgo crítico, propón 2 acciones 
   concretas de mejora que sean:
   - Específicas (qué hacer exactamente)
   - Medibles (cómo saber si funcionó)
   - Realizables en un plazo de 90 días

3. FORMATO: Presenta la información con la siguiente estructura para 
   cada hallazgo:
   
   ### Hallazgo [N]: [Título]
   - **Urgencia:** [Alta/Media-Alta/Media]
   - **Evidencia:** [Citar 2-3 comentarios específicos por número]
   - **Impacto potencial:** [Descripción breve del riesgo]
   - **Acción 1:** [Descripción + métrica de éxito + plazo]
   - **Acción 2:** [Descripción + métrica de éxito + plazo]

Sé directo y ejecutivo. Este documento será leído por directivos 
que necesitan tomar decisiones rápidas.
```

2. Revisa la respuesta de Copilot Chat. Verifica que contenga:
   - Exactamente 3 hallazgos priorizados
   - Evidencia citada con números de comentario específicos
   - 2 acciones por hallazgo con métricas y plazos

3. Si algún hallazgo te parece poco relevante o las acciones son demasiado genéricas, refina con un prompt adicional:

```
El hallazgo [N] necesita acciones más específicas. En lugar de 
"mejorar la comunicación", propón una solución tecnológica o de 
proceso concreta que Distribuidora Andina pueda implementar en 
30 días con recursos existentes.
```

4. Copia la respuesta final completa de Copilot Chat (la síntesis ejecutiva con los 3 hallazgos y sus acciones).

**Output esperado:** Síntesis ejecutiva estructurada con 3 hallazgos priorizados. Ejemplo de hallazgo esperado:

> ### Hallazgo 1: Fallas sistemáticas en comunicación proactiva con clientes
> - **Urgencia:** Alta
> - **Evidencia:** Comentarios 05, 10, 19, 25, 28 — los clientes reportan no recibir notificaciones de despacho, retrasos ni estado de pedidos
> - **Impacto potencial:** Pérdida de confianza y migración a competidores con mejor trazabilidad
> - **Acción 1:** Implementar notificaciones automáticas por correo/SMS en cada cambio de estado del pedido. Métrica: 100% de pedidos con al menos 3 notificaciones automáticas. Plazo: 60 días.
> - **Acción 2:** Crear portal web de rastreo de pedidos en tiempo real para clientes. Métrica: 80% de clientes activos registrados en el portal. Plazo: 90 días.

**Verificación:**
- [ ] La respuesta contiene exactamente 3 hallazgos priorizados
- [ ] Cada hallazgo cita números de comentario específicos como evidencia
- [ ] Cada hallazgo incluye 2 acciones con métricas y plazos definidos
- [ ] Los hallazgos están ordenados por urgencia (Alta → Media-Alta → Media)
- [ ] Las acciones son específicas y realizables, no genéricas

---

### Paso 6: Crear el documento consolidado final

**Objetivo:** Integrar todos los outputs del batch (Labs 04-02-01, 04-03-01 y 04-04-01) en un reporte ejecutivo unificado que demuestre el flujo de trabajo encadenado.

**Instrucciones:**

1. Regresa a OneDrive (`https://onedrive.live.com` o desde el portal Microsoft 365).
2. Navega a la carpeta `Copilot_Labs`.
3. Haz clic en **+ Nuevo** → **Documento de Word**.
4. Renombra el archivo como `Reporte_Final_Auditoria_DistribuidoraAndina.docx`.
5. Estructura el documento con las siguientes secciones. Escribe los encabezados y contenido según se indica:

**Sección 1 — Portada:**
```
REPORTE FINAL DE AUDITORÍA INTERNA
Distribuidora Andina S.A.
Análisis de Experiencia del Cliente — Q1 2025

Preparado por: [Tu nombre]
Fecha: [Fecha actual]
Herramienta utilizada: Microsoft 365 Copilot Chat

---

Este documento consolida los resultados de tres fases de trabajo 
asistido por IA generativa:
• Fase 1: Plan de auditoría interna (Lab 04-02-01)
• Fase 2: Infografía ejecutiva del plan (Lab 04-03-01)
• Fase 3: Análisis de comentarios de clientes (Lab 04-04-01)
```

6. **Sección 2 — Resumen del Plan de Auditoría:** Abre en otra pestaña el archivo `Plan_Auditoria_DistribuidoraAndina.docx`. Copia el Resumen Ejecutivo (o los primeros 2-3 párrafos que describen el plan) y pégalo en esta sección del reporte final bajo el encabezado:

```
## 1. Plan de Auditoría Interna (Referencia: Lab 04-02-01)

[Pegar aquí el resumen ejecutivo del plan de auditoría]
```

7. **Sección 3 — Infografía Ejecutiva:** Inserta la imagen de la infografía:
   - Coloca el cursor debajo del encabezado de la Sección 3
   - Haz clic en **Insertar** → **Imagen** → **Desde OneDrive**
   - Selecciona `Infografia_Auditoria_DistribuidoraAndina.png`
   - Ajusta el tamaño a ancho de página

```
## 2. Infografía Ejecutiva del Plan de Auditoría (Referencia: Lab 04-03-01)

[Imagen insertada aquí]
```

8. **Sección 4 — Análisis de Comentarios:** Pega la tabla de categorización del Paso 2 y la síntesis ejecutiva del Paso 5:

```
## 3. Análisis de Comentarios de Clientes (Referencia: Lab 04-04-01)

### 3.1 Categorización Temática
[Pegar tabla de categorías y frecuencias del Paso 2]

### 3.2 Visualizaciones
[Insertar Grafico_Temas_Clientes.png]
[Insertar Grafico_Sentimientos_Clientes.png]

### 3.3 Hallazgos Priorizados y Acciones de Mejora
[Pegar la síntesis ejecutiva completa del Paso 5]
```

9. Inserta las imágenes de los gráficos:
   - **Insertar** → **Imagen** → **Desde OneDrive** → selecciona `Grafico_Temas_Clientes.png`
   - Repite para `Grafico_Sentimientos_Clientes.png`

10. **Sección 5 — Conclusión:** Agrega un párrafo final:

```
## 4. Conclusión y Reflexión sobre el Proceso

Este reporte demuestra cómo Microsoft 365 Copilot Chat puede utilizarse 
como herramienta de productividad ejecutiva para:
- Planificar procesos complejos (auditoría interna)
- Comunicar visualmente planes y estrategias (infografía)
- Analizar datos cualitativos y generar insights accionables (análisis de comentarios)

El flujo encadenado de los tres laboratorios simula un ciclo completo de 
trabajo con IA corporativa: desde la planificación hasta el análisis y 
la propuesta de mejoras concretas.
```

11. Guarda el documento y verifica que todos los elementos estén correctamente insertados.

**Output esperado:** Documento Word de 4-6 páginas con portada, resumen del plan de auditoría, infografía insertada, tabla de análisis, dos gráficos insertados, síntesis ejecutiva con acciones de mejora y conclusión.

**Verificación:**
- [ ] El documento `Reporte_Final_Auditoria_DistribuidoraAndina.docx` existe en `Copilot_Labs`
- [ ] Contiene las 5 secciones especificadas
- [ ] Las 2 imágenes de gráficos están insertadas y son visibles
- [ ] La infografía del Lab 04-03-01 está insertada
- [ ] El contenido del Lab 04-02-01 está referenciado/incluido
- [ ] El documento demuestra claramente la integración de los 3 laboratorios

---

## Validación y pruebas

Completa la siguiente lista de verificación para confirmar que has cumplido todos los objetivos del laboratorio:

| # | Criterio de validación | Estado |
|---|------------------------|--------|
| 1 | `Comentarios_Clientes_DistribuidoraAndina.docx` contiene 30 comentarios numerados | ☐ |
| 2 | Copilot Chat identificó 5 categorías temáticas con frecuencias | ☐ |
| 3 | `Grafico_Temas_Clientes.png` descargado y guardado en `Copilot_Labs` | ☐ |
| 4 | `Grafico_Sentimientos_Clientes.png` descargado y guardado en `Copilot_Labs` | ☐ |
| 5 | Síntesis ejecutiva contiene 3 hallazgos con acciones medibles | ☐ |
| 6 | `Reporte_Final_Auditoria_DistribuidoraAndina.docx` integra outputs de 3 labs | ☐ |
| 7 | Todos los archivos están en la carpeta `Copilot_Labs` de OneDrive | ☐ |

**Prueba de integración:** Abre el reporte final y verifica que un lector sin contexto previo pueda entender:
- Qué se auditó y por qué
- Qué dicen los clientes (datos)
- Cuáles son los problemas prioritarios (análisis)
- Qué se propone hacer al respecto (acciones)

---

## Solución de problemas

### Problema 1: Copilot Chat no genera imágenes de gráficos

**Síntomas:** Al solicitar un gráfico, Copilot Chat responde con una descripción textual del gráfico, genera código Python/matplotlib, o indica que no puede crear imágenes.

**Causa:** La capacidad de generación de imágenes en Copilot Chat depende de la configuración del tenant y la versión del servicio. Algunos tenants tienen deshabilitada la generación de imágenes por política del administrador, o el modelo puede interpretar la solicitud como una petición de código en lugar de una imagen.

**Solución:**
1. Reformula el prompt agregando explícitamente: "Genera esto como una imagen visual que yo pueda descargar directamente. No quiero código ni descripción textual, quiero la imagen renderizada."
2. Si persiste, intenta: "Usa tu capacidad de creación de imágenes (como Designer) para generar un gráfico de barras con estos datos: [lista los datos explícitamente]."
3. **Plan B:** Si el tenant definitivamente no soporta generación de imágenes, copia los datos tabulares que Copilot generó, abre Excel Online, crea un gráfico manualmente con esos datos, y expórtalo como imagen (clic derecho en el gráfico → "Guardar como imagen"). Documenta en tu reporte que usaste este método alternativo.

---

### Problema 2: Copilot Chat no puede leer el archivo adjunto de Word

**Síntomas:** Al adjuntar `Comentarios_Clientes_DistribuidoraAndina.docx`, Copilot Chat responde con "No puedo acceder al archivo", "No se encontró contenido relevante" o genera un análisis que no corresponde a los 30 comentarios.

**Causa:** El archivo puede no haberse sincronizado completamente con OneDrive, el formato del documento puede incluir elementos que interfieren con la lectura (tablas complejas, imágenes), o la funcionalidad de adjuntar archivos puede tener restricciones en el tenant.

**Solución:**
1. Verifica que el archivo esté completamente sincronizado: abre OneDrive en el navegador y confirma que el archivo muestra la fecha de modificación reciente.
2. Abre el archivo Word, selecciona todo el texto (Ctrl+A), cópialo (Ctrl+C).
3. En Copilot Chat, pega el contenido directamente en el cuadro de mensaje (Ctrl+V) seguido del prompt de análisis.
4. Si el texto es demasiado largo para un solo mensaje, divídelo: pega los comentarios 01-15 con la instrucción "Estos son los primeros 15 de 30 comentarios. Espera al siguiente mensaje para los restantes." Luego envía los comentarios 16-30 con: "Aquí están los comentarios 16-30. Ahora analiza el conjunto completo de 30."

---

## Limpieza

No se requiere eliminar archivos al finalizar este laboratorio. Todos los archivos generados forman parte del entregable final del batch y deben permanecer en la carpeta `Copilot_Labs` para revisión del instructor.

**Verificación final de archivos en `Copilot_Labs`:**

```
✓ Plan_Auditoria_DistribuidoraAndina.docx          (Lab 04-02-01)
✓ Infografia_Auditoria_DistribuidoraAndina.png      (Lab 04-03-01)
✓ Comentarios_Clientes_DistribuidoraAndina.docx     (Lab 04-04-01)
✓ Grafico_Temas_Clientes.png                        (Lab 04-04-01)
✓ Grafico_Sentimientos_Clientes.png                  (Lab 04-04-01)
✓ Reporte_Final_Auditoria_DistribuidoraAndina.docx  (Lab 04-04-01)
```

Si deseas limpiar el historial de conversación de Copilot Chat, puedes hacerlo desde el menú de actividad reciente, pero no es obligatorio.

---

## Resumen

En este laboratorio completaste un ciclo completo de análisis cualitativo asistido por IA:

| Fase | Actividad realizada | Técnica de prompting aplicada |
|------|--------------------|-----------------------------|
| Preparación | Creación de archivo estructurado con 30 comentarios | Formato limpio y numerado para optimizar lectura por IA |
| Fase 1 | Identificación de temas y frecuencias | Prompt de análisis con contexto, tarea específica y formato de salida definido |
| Fase 2 | Generación de gráfico de barras | Prompt de visualización con especificaciones de diseño |
| Fase 3 | Generación de gráfico circular | Prompt de visualización con validación previa de datos |
| Fase 4 | Priorización y acciones de mejora | Prompt de síntesis ejecutiva con criterios de calidad (específico, medible, con plazo) |
| Consolidación | Reporte integrado de 3 laboratorios | Demostración de flujo encadenado de trabajo con IA |

**Conceptos clave reforzados:**
- La **progresión iterativa de prompts** (general → específico → estratégico) produce análisis más ricos que una sola solicitud
- Los **prompts de visualización** requieren especificaciones claras de formato, colores y estilo
- El **refinamiento** permite pasar de hallazgos descriptivos a propuestas accionables
- El **encadenamiento de outputs** entre laboratorios simula un flujo real de trabajo corporativo con IA

### Recursos adicionales

- Documentación oficial: [Microsoft Copilot Chat - Análisis de documentos](https://support.microsoft.com/copilot)
- Guía de prompt engineering para análisis de datos: Módulo teórico 4.4 del curso
- Plantilla de reporte ejecutivo: disponible en `OneDrive > Curso-M365-Copilot > Recursos-Compartidos`
