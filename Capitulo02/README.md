# Práctica guiada: Transformar una descripción textual en una imagen generada por Copilot Chat

## Metadata

| Campo | Detalle |
|-------|---------|
| **Duración** | 40 minutos |
| **Complejidad** | Fácil |
| **Nivel Bloom** | Aplicar |
| **Módulo** | 2.3 — De una idea a una pieza visual con IA |
| **Escenario** | Contoso Corp — Comunicación interna sobre política de trabajo híbrido |

---

## Descripción General

En este laboratorio transformarás una necesidad de comunicación visual corporativa en una imagen generada por inteligencia artificial utilizando Copilot Chat. Partiendo del escenario de Contoso Corp y su política de trabajo híbrido (establecido en el Lab 01-03-01), redactarás prompts de imagen estructurados, generarás múltiples variantes visuales, evaluarás su adecuación al propósito comunicativo y guardarás la imagen final para su uso posterior en la presentación ejecutiva del Lab 03-02-01.

---

## Objetivos de Aprendizaje

Al completar este laboratorio serás capaz de:

- [ ] Identificar una necesidad de comunicación visual corporativa y documentarla mediante la Ficha de Necesidad Visual
- [ ] Redactar un prompt de imagen estructurado en cuatro capas (sujeto, entorno/composición, estilo/atmósfera, especificaciones técnicas) para Copilot Chat
- [ ] Generar al menos dos variantes de imagen modificando elementos clave del prompt y observando cómo los cambios afectan el resultado
- [ ] Evaluar las imágenes generadas según criterios de adecuación al propósito comunicativo, alineación con marca corporativa y calidad visual
- [ ] Guardar la imagen seleccionada en OneDrive con nomenclatura estandarizada para su reutilización en laboratorios posteriores

---

## Prerrequisitos

### Conocimientos previos

| Requisito | Verificación |
|-----------|-------------|
| Laboratorio 01-03-01 completado | Tienes el contexto del escenario Contoso Corp disponible |
| Familiaridad con la interfaz de Copilot Chat | Has navegado y enviado al menos un prompt textual en copilot.microsoft.com |
| Comprensión del escenario Contoso Corp | Conoces: empresa de tecnología, 500 empleados, política híbrida 3+2, datos de satisfacción |

### Acceso y herramientas

| Recurso | Estado requerido |
|---------|-----------------|
| Cuenta corporativa Microsoft 365 con licencia Copilot | Activa y verificada |
| Acceso a copilot.microsoft.com | Protección de datos comerciales visible |
| Función de generación de imágenes en Copilot Chat | Habilitada (integración con Microsoft Designer) |
| Carpeta `OneDrive\Curso-M365-Copilot\Lab02\` | Creada y sincronizada |
| Archivo `Contexto-Contoso-Corp.pdf` | Disponible en `OneDrive\Curso-M365-Copilot\Recursos-Compartidos\` |

---

## Entorno del Laboratorio

### Hardware mínimo

| Componente | Especificación |
|------------|---------------|
| Procesador | Intel Core i5 8ª gen. o AMD Ryzen 5 3000+ (64 bits) |
| RAM | 8 GB mínimo |
| Almacenamiento disponible | 2 GB para archivos de práctica e imágenes |
| Conexión a Internet | 10 Mbps de descarga mínimo |
| Periféricos | Teclado, ratón/trackpad |

### Software requerido

| Aplicación | Versión / Acceso |
|------------|-----------------|
| Microsoft Edge | 124.0.2478.105 o superior |
| Microsoft Copilot Chat (web) | copilot.microsoft.com — con Commercial Data Protection |
| Microsoft Designer | Integrado en Copilot Chat (no requiere acceso independiente) |
| OneDrive for Business | Cliente de sincronización 24.071.0407.0003+ |

### Verificación inicial del entorno

Antes de comenzar, ejecuta estas comprobaciones:

1. Abre Microsoft Edge y navega a `https://copilot.microsoft.com`
2. Inicia sesión con tu cuenta corporativa (`usuario@contoso-curso.onmicrosoft.com`)
3. Confirma que aparece el mensaje: **"Tu organización tiene protección de datos comerciales activada"**
4. Verifica que la carpeta `OneDrive\Curso-M365-Copilot\Lab02\` existe en tu explorador de archivos

> ⚠️ **IMPORTANTE:** Si no ves el mensaje de protección de datos comerciales, NO continúes. Notifica al instructor para verificar tu asignación de licencia.

---

## Procedimiento Paso a Paso

### Paso 1: Definir la necesidad de comunicación visual

**Objetivo:** Identificar y documentar la necesidad visual específica para el escenario de Contoso Corp utilizando la Ficha de Necesidad Visual.

**Instrucciones:**

1. Abre el archivo `Contexto-Contoso-Corp.pdf` desde `OneDrive\Curso-M365-Copilot\Recursos-Compartidos\` para refrescar el contexto del escenario.

2. Recuerda los datos clave del escenario:
   - **Empresa:** Contoso Corp (tecnología, 500 empleados)
   - **Política:** Trabajo híbrido — 3 días presencial, 2 días remoto
   - **Satisfacción:** 72% satisfechos, 18% neutrales, 10% insatisfechos
   - **Necesidad:** Comunicar internamente esta política de forma visual y atractiva

3. Abre un documento de texto nuevo (puedes usar el Bloc de notas o cualquier editor) y completa la siguiente **Ficha de Necesidad Visual**:

```
═══════════════════════════════════════════════════════
FICHA DE NECESIDAD VISUAL — Lab 02-03-01
═══════════════════════════════════════════════════════

¿Para qué sirve esta imagen?
→ Banner/portada para el comunicado interno sobre la política de trabajo híbrido de Contoso Corp

¿Quién la verá?
→ Los 500 empleados de Contoso Corp (audiencia interna diversa: técnicos, administrativos, directivos)

¿Dónde se usará?
→ Encabezado de comunicado en intranet, portada de presentación ejecutiva (Lab 03-02-01), posible inclusión en correo electrónico masivo

¿Qué mensaje debe transmitir?
→ Flexibilidad, colaboración y equilibrio entre trabajo presencial y remoto; modernidad y confianza en el modelo híbrido

¿Qué estilo visual es apropiado?
→ Corporativo moderno, limpio, profesional pero accesible; no demasiado formal ni demasiado informal

¿Hay restricciones de marca?
→ Paleta corporativa de Contoso: azul primario #0078D4, blanco #FFFFFF, gris oscuro #323130. Tipografía Segoe UI. Sin texto dentro de la imagen (el texto se añadirá por separado).

═══════════════════════════════════════════════════════
```

4. Guarda este archivo como `Ficha-Necesidad-Visual.txt` en `OneDrive\Curso-M365-Copilot\Lab02\`.

**Resultado esperado:** Un archivo de texto con la ficha completada que documenta claramente la audiencia, contexto, mensaje, estilo y restricciones de la imagen a generar.

**Verificación:**
- [ ] La ficha contiene respuestas específicas en los 6 campos
- [ ] El mensaje central está enfocado en un concepto claro (trabajo híbrido/flexibilidad)
- [ ] Las restricciones de marca incluyen los colores corporativos de Contoso (#0078D4, #FFFFFF, #323130)
- [ ] El archivo está guardado en la carpeta Lab02

---

### Paso 2: Redactar el primer prompt de imagen (Variante A)

**Objetivo:** Construir un prompt de imagen estructurado en cuatro capas que traduzca la necesidad visual documentada en una descripción interpretable por Copilot Chat.

**Instrucciones:**

1. Con la Ficha de Necesidad Visual abierta como referencia, construye tu prompt aplicando la estructura de cuatro capas:

   **Capa 1 — Sujeto principal:** ¿Qué elemento central debe aparecer?
   
   **Capa 2 — Entorno y composición:** ¿Cómo se organiza la escena?
   
   **Capa 3 — Estilo y atmósfera:** ¿Qué sensación visual debe transmitir?
   
   **Capa 4 — Especificaciones técnicas:** ¿Qué restricciones de formato y color aplican?

2. Redacta el siguiente prompt (Variante A) — puedes copiarlo directamente o adaptarlo ligeramente según tu interpretación:

```
Variante A — Estilo ilustración corporativa:

Crea una ilustración vectorial de estilo corporativo moderno que represente 
el concepto de trabajo híbrido. La composición muestra en el centro una 
figura humana estilizada conectada por líneas suaves a dos entornos: a la 
izquierda, un espacio de oficina moderno con escritorios colaborativos y 
una ventana luminosa; a la derecha, un espacio de home office acogedor con 
una laptop, una planta y una taza de café. Ambos entornos están conectados 
por una línea curva que sugiere fluidez y continuidad. Estilo minimalista 
y profesional, atmósfera positiva y moderna, sensación de equilibrio y 
flexibilidad. Paleta de colores: azul (#0078D4) como color dominante, 
blanco (#FFFFFF) como fondo, acentos en gris oscuro (#323130). Formato 
horizontal 16:9. Sin texto en la imagen.
```

3. Abre `copilot.microsoft.com` en Microsoft Edge (si no está ya abierto).

4. Confirma visualmente que la protección de datos comerciales está activa.

5. Copia y pega el prompt de la Variante A en el campo de entrada de Copilot Chat.

6. Presiona **Enter** o haz clic en el botón de enviar.

7. Espera a que Copilot genere la imagen (normalmente entre 10 y 30 segundos).

**Resultado esperado:** Copilot Chat genera una o varias imágenes basadas en tu descripción. La imagen debería mostrar elementos relacionados con trabajo híbrido (oficina y hogar) con predominancia del color azul corporativo y un estilo limpio/moderno.

**Verificación:**
- [ ] Copilot generó al menos una imagen visible en la conversación
- [ ] La imagen refleja elementos de trabajo híbrido (oficina + hogar/remoto)
- [ ] El estilo visual es corporativo/profesional (no caricaturesco ni fotorrealista extremo)
- [ ] Los tonos azules son predominantes en la composición

> 💡 **Nota:** La IA generativa produce resultados variables. Tu imagen no será idéntica a la de otros participantes, y eso es esperado. Lo importante es evaluar si cumple con el propósito comunicativo definido.

---

### Paso 3: Generar una segunda variante modificando el estilo (Variante B)

**Objetivo:** Observar cómo la modificación del estilo artístico en el prompt produce resultados visuales significativamente diferentes, manteniendo el mismo mensaje central.

**Instrucciones:**

1. En la misma conversación de Copilot Chat, redacta un nuevo prompt que mantenga el mismo sujeto y mensaje pero cambie el estilo visual a **fotografía conceptual**:

```
Variante B — Estilo fotografía conceptual:

Genera una imagen en estilo de fotografía de stock profesional que 
represente el trabajo híbrido moderno. La escena muestra una vista 
dividida en dos mitades armoniosas: la mitad izquierda es una oficina 
corporativa luminosa con paredes de cristal, escritorios limpios y luz 
natural entrando por grandes ventanales; la mitad derecha es un espacio 
doméstico elegante con una laptop abierta sobre un escritorio de madera, 
una ventana con vista a un jardín y elementos de confort (planta, café). 
La transición entre ambos espacios es suave y fluida, sin una línea 
divisoria dura. Iluminación cálida y profesional. Tonos predominantes: 
azul corporativo y blanco con toques de gris. Composición horizontal 
16:9. Aspecto moderno y optimista. Sin personas con rostros visibles. 
Sin texto en la imagen.
```

2. Pega este prompt en Copilot Chat y envíalo.

3. Espera la generación de la imagen (10-30 segundos).

4. Observa las diferencias fundamentales entre la Variante A (ilustración vectorial) y la Variante B (fotografía conceptual):
   - ¿Cuál transmite más profesionalismo?
   - ¿Cuál es más versátil para diferentes usos?
   - ¿Cuál se alinea mejor con el tono de comunicación interna de Contoso?

**Resultado esperado:** Una imagen con estilo fotográfico/fotorrealista que muestra espacios de trabajo (oficina y hogar) con una estética más realista que la Variante A, manteniendo la paleta azul/blanco/gris.

**Verificación:**
- [ ] La imagen tiene un estilo claramente diferente a la Variante A
- [ ] Se percibe un estilo fotográfico o fotorrealista (no ilustración plana)
- [ ] El concepto de trabajo híbrido (dos espacios) sigue siendo reconocible
- [ ] La paleta de colores mantiene coherencia con la marca Contoso

---

### Paso 4: Generar una tercera variante con ajuste de composición (Variante C)

**Objetivo:** Practicar el refinamiento iterativo de prompts modificando la composición y los elementos visuales para explorar una tercera dirección creativa.

**Instrucciones:**

1. Para esta tercera variante, cambiaremos tanto el enfoque conceptual como la composición. En lugar de mostrar dos espacios divididos, usaremos una **metáfora visual abstracta** del equilibrio:

```
Variante C — Estilo abstracto/metafórico:

Crea una imagen de estilo gráfico corporativo abstracto que represente 
la flexibilidad del trabajo híbrido mediante una metáfora visual. La 
composición muestra formas geométricas suaves (círculos y rectángulos 
redondeados) flotando en equilibrio dinámico, como un móvil de Calder. 
Algunas formas contienen íconos minimalistas de oficina (edificio, 
pantalla de computadora, personas reunidas) y otras contienen íconos de 
trabajo remoto (casa, wifi, laptop, reloj flexible). Las formas están 
conectadas por líneas delgadas y elegantes que sugieren red y conexión. 
Fondo blanco limpio con abundante espacio negativo. Color principal: 
azul #0078D4. Colores secundarios: gris claro y blanco. Estilo ultra 
limpio y sofisticado, apropiado para una presentación ejecutiva de alto 
nivel. Formato horizontal 16:9. Sin texto en la imagen.
```

2. Envía el prompt en Copilot Chat.

3. Una vez generada la imagen, compara mentalmente las tres variantes:

| Criterio | Variante A (Ilustración) | Variante B (Fotografía) | Variante C (Abstracto) |
|----------|--------------------------|------------------------|----------------------|
| Claridad del mensaje | | | |
| Profesionalismo | | | |
| Versatilidad de uso | | | |
| Alineación con marca Contoso | | | |
| Impacto visual | | | |

4. Anota tus observaciones brevemente en un nuevo archivo de texto o al final de tu `Ficha-Necesidad-Visual.txt`.

**Resultado esperado:** Una imagen de estilo más abstracto/geométrico con formas y líneas que representan conceptualmente la conexión entre trabajo presencial y remoto, con predominancia del azul #0078D4 sobre fondo blanco.

**Verificación:**
- [ ] La imagen tiene un estilo claramente diferente a las variantes A y B
- [ ] El estilo es más abstracto/geométrico que las variantes anteriores
- [ ] La paleta de colores se mantiene dentro de los tonos corporativos de Contoso
- [ ] Has documentado una comparación breve entre las tres variantes

---

### Paso 5: Seleccionar y descargar la imagen final

**Objetivo:** Evaluar las variantes generadas con criterios objetivos, seleccionar la más adecuada y guardarla con la nomenclatura correcta para uso en laboratorios posteriores.

**Instrucciones:**

1. Revisa las tres (o más) imágenes generadas en tu conversación de Copilot Chat. Aplica los siguientes **criterios de evaluación**:

   | Criterio | Peso | Pregunta clave |
   |----------|------|---------------|
   | Adecuación al mensaje | Alto | ¿Comunica "trabajo híbrido flexible" de forma clara? |
   | Alineación con marca | Alto | ¿Respeta la paleta azul/blanco/gris de Contoso? |
   | Calidad visual | Medio | ¿Se ve profesional y bien compuesta? ¿Hay artefactos visuales? |
   | Versatilidad | Medio | ¿Funciona tanto como banner en intranet como en portada de presentación? |
   | Ausencia de texto | Bajo | ¿La imagen está libre de texto generado por la IA? |

2. Selecciona la imagen que mejor cumple con estos criterios. Si ninguna te satisface completamente, puedes generar una variante adicional refinando el prompt de tu favorita (esto es opcional y depende del tiempo disponible).

3. Para descargar la imagen seleccionada:
   - Haz clic en la imagen generada dentro de Copilot Chat para ampliarla
   - Busca el botón de **descarga** (ícono de flecha hacia abajo) o haz clic derecho y selecciona **"Guardar imagen como..."**
   - Si Copilot ofrece la opción de abrir en Microsoft Designer, también puedes hacerlo para obtener opciones de descarga adicionales

4. Guarda la imagen con el nombre exacto: `Banner-Hibrido-Final.png`

5. Ubica el archivo en la ruta: `OneDrive\Curso-M365-Copilot\Lab02\Banner-Hibrido-Final.png`

6. Adicionalmente, guarda al menos una de las variantes no seleccionadas con un nombre descriptivo, por ejemplo:
   - `Variante-A-Ilustracion.png`
   - `Variante-B-Fotografia.png`
   - `Variante-C-Abstracto.png`

7. Verifica que los archivos se sincronicen correctamente con OneDrive (el ícono de nube con checkmark verde debe aparecer junto a cada archivo).

**Resultado esperado:** Al menos dos archivos de imagen guardados en `OneDrive\Curso-M365-Copilot\Lab02\`, incluyendo obligatoriamente `Banner-Hibrido-Final.png`.

**Verificación:**
- [ ] El archivo `Banner-Hibrido-Final.png` existe en `OneDrive\Curso-M365-Copilot\Lab02\`
- [ ] Al menos un archivo adicional de variante está guardado en la misma carpeta
- [ ] Los archivos están sincronizados con OneDrive (checkmark verde visible)
- [ ] La imagen final seleccionada cumple con los criterios de evaluación documentados

---

### Paso 6: Documentar el proceso y los prompts utilizados

**Objetivo:** Crear un registro de los prompts utilizados y las decisiones tomadas, generando un recurso reutilizable para futuros proyectos de generación de imágenes.

**Instrucciones:**

1. Crea un nuevo archivo de texto llamado `Registro-Prompts-Imagenes.txt` en `OneDrive\Curso-M365-Copilot\Lab02\`.

2. Documenta el contenido siguiente (puedes copiar la estructura y completar con tus datos):

```
═══════════════════════════════════════════════════════
REGISTRO DE PROMPTS DE IMAGEN — Lab 02-03-01
Fecha: [Tu fecha]
Participante: [Tu nombre]
═══════════════════════════════════════════════════════

CONTEXTO:
- Escenario: Contoso Corp — Política de trabajo híbrido
- Propósito: Banner para comunicado interno
- Uso posterior: Portada de presentación ejecutiva (Lab 03-02-01)

───────────────────────────────────────────────────────
VARIANTE A — Ilustración corporativa
───────────────────────────────────────────────────────
Prompt utilizado:
[Pegar aquí el prompt exacto de la Variante A]

Resultado obtenido:
[Describir brevemente qué generó la IA - 2 a 3 oraciones]

Evaluación:
- Adecuación al mensaje: [Alta/Media/Baja]
- Alineación con marca: [Alta/Media/Baja]
- Calidad visual: [Alta/Media/Baja]

───────────────────────────────────────────────────────
VARIANTE B — Fotografía conceptual
───────────────────────────────────────────────────────
Prompt utilizado:
[Pegar aquí el prompt exacto de la Variante B]

Resultado obtenido:
[Describir brevemente qué generó la IA - 2 a 3 oraciones]

Evaluación:
- Adecuación al mensaje: [Alta/Media/Baja]
- Alineación con marca: [Alta/Media/Baja]
- Calidad visual: [Alta/Media/Baja]

───────────────────────────────────────────────────────
VARIANTE C — Abstracto/metafórico
───────────────────────────────────────────────────────
Prompt utilizado:
[Pegar aquí el prompt exacto de la Variante C]

Resultado obtenido:
[Describir brevemente qué generó la IA - 2 a 3 oraciones]

Evaluación:
- Adecuación al mensaje: [Alta/Media/Baja]
- Alineación con marca: [Alta/Media/Baja]
- Calidad visual: [Alta/Media/Baja]

───────────────────────────────────────────────────────
DECISIÓN FINAL
───────────────────────────────────────────────────────
Variante seleccionada: [A / B / C / Otra]
Justificación: [Explicar en 2-3 oraciones por qué esta variante 
es la más adecuada para el propósito definido]

Archivo guardado como: Banner-Hibrido-Final.png

───────────────────────────────────────────────────────
LECCIONES APRENDIDAS
───────────────────────────────────────────────────────
1. [Qué funcionó bien en tus prompts]
2. [Qué cambiarías la próxima vez]
3. [Qué descubriste sobre la generación de imágenes con IA]

═══════════════════════════════════════════════════════
```

3. Guarda el archivo completado.

**Resultado esperado:** Un archivo de registro completo que documenta los tres prompts, los resultados obtenidos, las evaluaciones y la justificación de la selección final.

**Verificación:**
- [ ] El archivo `Registro-Prompts-Imagenes.txt` existe en `OneDrive\Curso-M365-Copilot\Lab02\`
- [ ] Contiene los tres prompts utilizados (o los que hayas generado)
- [ ] Incluye evaluaciones para cada variante
- [ ] Documenta la justificación de la selección final
- [ ] Incluye al menos una lección aprendida

---

## Validación y Pruebas

Al finalizar el laboratorio, verifica que cumples con **todos** los siguientes criterios de éxito:

### Lista de verificación final

| # | Criterio | ¿Cumplido? |
|---|----------|:----------:|
| 1 | La Ficha de Necesidad Visual está completa con los 6 campos respondidos | ☐ |
| 2 | Se generaron al menos 2 variantes de imagen con prompts distintos | ☐ |
| 3 | Los prompts utilizan la estructura de 4 capas (sujeto, entorno, estilo, especificaciones) | ☐ |
| 4 | La imagen final refleja el concepto de trabajo híbrido de Contoso Corp | ☐ |
| 5 | La paleta de colores de la imagen se aproxima a los tonos corporativos (#0078D4, blanco, gris) | ☐ |
| 6 | El archivo `Banner-Hibrido-Final.png` existe en `OneDrive\Curso-M365-Copilot\Lab02\` | ☐ |
| 7 | Al menos una variante adicional está guardada en la misma carpeta | ☐ |
| 8 | El archivo `Registro-Prompts-Imagenes.txt` está completo y guardado | ☐ |
| 9 | Todos los archivos están sincronizados con OneDrive | ☐ |

### Prueba de integración con Lab 03-02-01

Para confirmar que tu imagen estará disponible para el siguiente laboratorio:

1. Navega a `OneDrive\Curso-M365-Copilot\Lab02\` en el explorador de archivos
2. Haz doble clic en `Banner-Hibrido-Final.png` para abrirla
3. Confirma que la imagen se abre correctamente y tiene calidad suficiente para una presentación (no está pixelada ni cortada)
4. Verifica que el formato es horizontal (más ancho que alto), ideal para uso como banner o portada de diapositiva

---

## Solución de Problemas

### Problema 1: Copilot Chat no genera imágenes

**Síntomas:** Al enviar el prompt de imagen, Copilot responde solo con texto (describe la imagen en palabras) o muestra un mensaje indicando que no puede generar imágenes.

**Causa:** La función de generación de imágenes (integración con Microsoft Designer/DALL-E) puede no estar habilitada para tu cuenta, o la licencia de Copilot asignada no incluye esta capacidad. También puede ocurrir si el tenant tiene restricciones administrativas sobre la generación de contenido visual.

**Solución:**
1. Verifica que estás en `copilot.microsoft.com` (no en bing.com/chat ni en otra URL)
2. Confirma que has iniciado sesión con tu cuenta corporativa (no personal)
3. Intenta reformular el prompt comenzando explícitamente con "Crea una imagen de..." o "Genera una imagen que muestre..."
4. Si el problema persiste, prueba acceder directamente a `designer.microsoft.com` con la misma cuenta corporativa para verificar si tienes acceso a Microsoft Designer
5. Notifica al instructor — puede ser necesario verificar la configuración de licencia o las políticas del tenant

### Problema 2: Las imágenes generadas contienen texto ilegible o no deseado

**Síntomas:** La imagen generada incluye palabras, letras o caracteres dentro de la composición visual que no fueron solicitados, o que aparecen con errores ortográficos y tipografía distorsionada.

**Causa:** Los modelos de generación de imágenes con IA frecuentemente interpretan elementos contextuales del prompt como solicitudes de incluir texto. Además, la generación de texto legible dentro de imágenes es una limitación conocida de los modelos actuales de IA generativa.

**Solución:**
1. Añade explícitamente al final de tu prompt la instrucción: `"Sin texto en la imagen. Sin palabras. Sin letras. Solo elementos visuales gráficos."`
2. Evita mencionar nombres de programas o títulos en el prompt (por ejemplo, no incluyas "con el título Trabajo Híbrido" en la descripción)
3. Si la imagen generada tiene texto no deseado pero el resto de la composición es buena, puedes:
   - Solicitar a Copilot: "Regenera la imagen anterior pero eliminando todo texto y letras"
   - Descargar la imagen y recortar la sección con texto usando cualquier editor de imágenes básico
4. Genera una nueva variante con el prompt corregido

---

## Limpieza

Este laboratorio **no requiere limpieza** de archivos, ya que los outputs generados serán utilizados en laboratorios posteriores:

- `Banner-Hibrido-Final.png` → Se usará en el Lab 03-02-01 (presentación PowerPoint)
- Los archivos de variantes y el registro de prompts son documentación de aprendizaje

**Acciones opcionales de organización:**
- Si generaste imágenes adicionales de prueba que no deseas conservar, puedes eliminarlas de la carpeta Lab02
- El historial de conversación en Copilot Chat se mantiene automáticamente y puede consultarse posteriormente

---

## Resumen

En este laboratorio has completado el ciclo completo de generación de contenido visual con IA corporativa:

| Fase | Actividad realizada | Habilidad desarrollada |
|------|-------------------|----------------------|
| 1. Identificación | Completaste la Ficha de Necesidad Visual | Análisis de requerimientos visuales |
| 2. Redacción | Construiste prompts en 4 capas | Comunicación estructurada con IA |
| 3. Generación | Produjiste 3+ variantes de imagen | Uso de Copilot Chat para contenido visual |
| 4. Evaluación | Comparaste variantes con criterios objetivos | Pensamiento crítico sobre outputs de IA |
| 5. Selección | Elegiste y guardaste la imagen final | Toma de decisiones basada en propósito |
| 6. Documentación | Registraste prompts y aprendizajes | Creación de recursos reutilizables |

### Conceptos clave para recordar

- **La claridad del propósito determina la calidad del resultado:** Completar la Ficha de Necesidad Visual antes de escribir cualquier prompt ahorra iteraciones innecesarias.
- **La estructura de 4 capas produce prompts efectivos:** Sujeto + Entorno/Composición + Estilo/Atmósfera + Especificaciones técnicas.
- **La iteración es parte del proceso:** Raramente la primera imagen generada es la definitiva. Generar variantes y comparar es la práctica estándar.
- **"Sin texto en la imagen"** es un modificador casi siempre necesario en prompts de imagen corporativa.

### Conexión con el siguiente laboratorio

El archivo `Banner-Hibrido-Final.png` que guardaste será insertado directamente en la presentación ejecutiva de PowerPoint que crearás en el **Lab 03-02-01**. Asegúrate de que permanece en `OneDrive\Curso-M365-Copilot\Lab02\` y está sincronizado.

### Recursos adicionales

- [Documentación oficial de Microsoft Designer](https://designer.microsoft.com)
- [Guía de prompts de imagen de Microsoft](https://support.microsoft.com/es-es/topic/crear-im%C3%A1genes-con-copilot)
- Archivo de referencia del curso: `Contexto-Contoso-Corp.pdf` en `Recursos-Compartidos\`

---
