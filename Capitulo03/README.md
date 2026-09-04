# Módulo 3 - Conversar mejor con la IA: solicitudes, contexto y refinamiento

# Práctica guiada: De información a una presentación alineada con la identidad corporativa

## Metadata

| Campo | Detalle |
|---|---|
| **Duración** | 14 minutos |
| **Complejidad** | Intermedia |
| **Nivel Bloom** | Aplicar / Analizar |
| **Módulo** | 3 - Conversar mejor con la IA: solicitudes, contexto y refinamiento |
| **Tecnología principal** | Copilot en PowerPoint |
| **Modalidad** | Demostración guiada |
| **Escenario** | Banco Horizonte - Resultados de un piloto de experiencia digital |

---

## Descripción General

En esta práctica crearás una presentación ejecutiva a partir de un informe empresarial ficticio y comprobarás cómo una plantilla corporativa ayuda a mantener consistencia visual. El archivo fuente incluye un brief con **contexto, objetivo, audiencia y expectativas**, además de los datos que deben utilizarse en las diapositivas.

Se proporcionan dos materiales porque representan artefactos habituales en una organización: un informe de resultados en Word y una plantilla de PowerPoint con identidad visual corporativa ficticia.

---

## Objetivos de Aprendizaje

Al completar esta práctica serás capaz de:

- [ ] Crear una presentación basada en un archivo fuente empresarial.
- [ ] Utilizar una plantilla o un Kit de marca disponible para mantener identidad visual.
- [ ] Validar que Copilot no altere cifras relevantes del documento fuente.
- [ ] Refinar una diapositiva mediante una instrucción concreta.

---

## Prerrequisitos

### Conocimientos previos

- Reconocer los componentes de una solicitud: contexto, objetivo, fuentes y expectativas.
- Saber abrir y guardar archivos de Word y PowerPoint en OneDrive.

### Acceso requerido

| Recurso | Estado requerido |
|---|---|
| Cuenta profesional o educativa de Microsoft 365 | Iniciada |
| Microsoft Copilot | Licencia de trabajo activa |
| Copilot en PowerPoint | Visible y habilitado |
| PowerPoint para Microsoft 365 | Web, Windows o Mac |
| OneDrive | Disponible para guardar los archivos |

> **Nota de funcionamiento:** Microsoft indica que, al crear una presentación referenciando un archivo, la creación se fundamenta en ese archivo y requiere revisión humana. Para hacer visible la lógica **contexto -> objetivo -> fuente -> expectativas** sin depender de una segunda entrada durante la generación, el documento del ejercicio incluye un brief de presentación al inicio.

---

## Entorno del Laboratorio

### Herramientas

- Microsoft Word o Word para la web.
- Microsoft PowerPoint para Microsoft 365.
- Copilot en PowerPoint.
- OneDrive.

### Materiales

Ubicados en `materiales/`:

1. `Informe_Resultados_Piloto_Experiencia_Digital.docx`
   - Informe ejecutivo ficticio que contiene el brief y los datos del piloto.
2. `Plantilla_Banco_Horizonte.pptx`
   - Plantilla ficticia con identidad visual azul/turquesa y diapositivas de muestra que Copilot puede utilizar como referencia de estilo.

---

## Procedimiento Paso a Paso

### Paso 1: Preparar los archivos

**Objetivo:** tener disponibles la fuente y la identidad visual antes de iniciar la generación.

**Instrucciones:**

1. Abre `materiales/Informe_Resultados_Piloto_Experiencia_Digital.docx`.
2. Lee únicamente la sección inicial **Brief de presentación** y ubica los cuatro elementos:
   - contexto;
   - objetivo;
   - audiencia;
   - expectativas.
3. Confirma que el documento contiene los resultados del piloto.
4. Carga ambos archivos a una carpeta de OneDrive.
5. Abre una presentación nueva en PowerPoint para Microsoft 365.


### Paso 2: Preparar la identidad visual

**Objetivo:** indicar a Copilot qué recursos de marca debe utilizar.

**Instrucciones:**

1. Abre el panel de **Copilot** en PowerPoint.
2. Si tu organización dispone de un Kit de marca autorizado, selecciona el botón **+** y luego **Seleccionar marca**.
3. Elige el Kit de marca autorizado.
4. Si no existe un Kit de marca, continúa con la plantilla `Plantilla_Banco_Horizonte.pptx`. La guía funciona utilizando la plantilla como referencia visual.

### Paso 3: Crear la presentación desde el archivo

**Objetivo:** generar una presentación fundamentada en el informe, no en información inventada.

**Instrucciones:**

1. En el panel de Copilot, solicita **Crear presentación desde archivo** o escribe:

```text
Crea una presentación a partir de /Informe_Resultados_Piloto_Experiencia_Digital.docx
```

2. Si PowerPoint abre un selector de archivos, selecciona `Informe_Resultados_Piloto_Experiencia_Digital.docx`.
3. Inicia la generación.
4. Si Copilot presenta un esquema antes de crear las diapositivas, confirma que se parece a esta secuencia:
   - propósito del piloto;
   - indicadores principales;
   - hallazgos;
   - acciones para 30 días;
   - decisión solicitada al comité.
5. Continúa con la creación de las diapositivas.


### Paso 4: Validar los datos antes de aceptar el resultado

**Objetivo:** comprobar que la presentación conserva los datos del archivo fuente.

**Instrucciones:** abre el Word en paralelo y verifica que la presentación mantenga exactamente estos valores:

| Indicador | Valor de control |
|---|---:|
| Satisfacción de usuarios del piloto | 89 % |
| Tiempo promedio de atención | 3,1 minutos |
| Resolución en primer contacto | 84 % |
| Interacciones analizadas | 1.200 |

Además comprueba que no aparezcan causas, porcentajes o conclusiones que no estén sustentados por el informe.

### Paso 5: Refinar una diapositiva

**Objetivo:** mejorar la comunicación visual sin cambiar el contenido factual.

**Instrucciones:** selecciona la diapositiva que contiene los indicadores y solicita:

```text
Refina esta diapositiva. Reduce el texto y presenta los indicadores principales como tarjetas visuales claras. Conserva exactamente los valores del documento fuente, no agregues nuevas métricas y mantén la identidad visual de la presentación.
```

Revisa el resultado y conserva la versión que mantenga cifras y legibilidad.

### Paso 6: Revisar la marca y guardar

**Instrucciones:**

**Objetivo:** confirmar que la presentación generada parece parte de un mismo sistema visual.

1. Recorre las miniaturas de las diapositivas.
2. Comprueba consistencia de tipografía, color, jerarquía y distribución.
3. Si la plantilla contenía diapositivas de ejemplo que no forman parte del resultado final, elimínalas únicamente después de que Copilot haya generado las nuevas diapositivas.
4. Guarda `Presentacion_Resultados_Piloto.pptx`.

![Generacion de presentacion](../imagenes/Capitulo3/1.png)
---

**Resultado esperado:** La presentación final conserva una apariencia consistente y queda guardada con el nombre indicado.

**Verificación:**

- [ ] Se revisaron tipografía, color, jerarquía y distribución.
- [ ] El archivo final fue guardado.

## Validación y Pruebas

- [ ] La presentación se generó a partir del informe Word suministrado.
- [ ] El informe contiene contexto, objetivo, audiencia y expectativas.
- [ ] Se utilizó una plantilla de marca o un Kit de marca disponible.
- [ ] Los cuatro valores de control coinciden con la fuente.
- [ ] Se realizó al menos un refinamiento de una diapositiva.
- [ ] La presentación mantiene una apariencia visual consistente.

---

## Solución de Problemas

### Copilot no aparece en PowerPoint

1. Comprueba que estás usando PowerPoint para Microsoft 365 con la cuenta de trabajo correcta.
2. Confirma que la organización tiene habilitado Copilot en PowerPoint.
3. Guarda el archivo en OneDrive y vuelve a abrirlo.

### No aparece **Seleccionar marca**

Continúa con la plantilla incluida. La administración de Kits de marca no forma parte de esta práctica.

### Copilot no encuentra el archivo Word

1. Confirma que el archivo está guardado en OneDrive.
2. Espera unos instantes después de subirlo.
3. Usa el botón de agregar contenido o escribe `/` en el cuadro de Copilot para localizar el archivo.

### Una cifra fue modificada

No aceptes el dato automáticamente. Corrige la diapositiva usando el valor de la fuente y conserva esa revisión como ejemplo de supervisión humana.

---

## Limpieza

Conserva los dos materiales originales. Puedes eliminar la presentación generada si fue creada únicamente para la práctica.

---

## Resumen

En catorce minutos transformaste un informe empresarial en una presentación, utilizaste recursos de marca, verificaste datos y refinaste una diapositiva. La práctica demuestra que una buena presentación con Copilot depende tanto de la calidad de la fuente y de las instrucciones como de la revisión humana posterior.

---

## Recursos adicionales

- Microsoft Support - Crear una presentación con Copilot en PowerPoint: https://support.microsoft.com/en-us/copilot-powerpoint
- Microsoft Support - Mantener la presentación alineada con la marca: https://support.microsoft.com/es-es/powerpoint/copilot/keep-your-presentation-on-brand-with-copilot
- Microsoft Support - Tutorial para crear una presentación de marca a partir de un archivo: https://support.microsoft.com/es-es/powerpoint/copilot-tutorial-create-a-branded-presentation-from-a-file
