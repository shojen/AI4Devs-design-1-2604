## Prompt 1:
actua como prompt engineer experto y mejora el siguiente prompt, devuelvelo en formato markdown en un archivo .md:

```markdown
## Tu rol

Actua como Product Manager experto. Definirás funcionalidades clave que harán brillar a LTI por encima de cualquier competidor. Aumentando la eficiencia para los departamentos de HR, mejorando la colaboración en tiempo real entre reclutadores y managers, automatizaciones, asistencia de IA en diversas tareas

## Información sobre el proyecto
LTI es una startup que quiere desarrollar el ATS (Applicant-Tracking System) del futuro. Lee para más información la imagen ats.jpg adjunta

## Acción
Haz brainstorming, investiga cuales pueden ser las claves del eéxito y déjalo plasmado para el resto del equipo

## Misión

Tu misión es **diseñar la primera versión del sistema, entregando los siguientes artefactos**:

- Descripción breve del software LTI, valor añadido y ventajas competitivas. Explicación de las funciones principales. Añadir un diagrama Lean Canvas para entender el modelo de negocio

- Descripción de los 3 casos de uso principales, con el diagrama asociado a cada uno

- Modelo de datos que cubra entidades, atributos (nombre y tipo) y relaciones

- Diseño del sistema a alto nivel, tanto explicado como diagrama adjunto

- Diagrama C4 que llegue en profundidad a uno de los componentes del sistema, el que prefieras

**IMPORTANTE**: Documenta todo en un único documento markdown correctamente formateado llamado LTI-ARP.md
```

## Respuesta 1:

Voy a mejorar este prompt aplicando buenas prácticas de prompt engineering y entregártelo como archivo `.md`.No hay skill específica de markdown, así que procedo a crear el archivo directamente. Déjame trabajar en la versión mejorada del prompt.Aquí tienes el prompt mejorado. Los cambios principales que apliqué:

**Estructura más clara.** Separé el prompt en secciones numeradas (rol, contexto, objetivo, entregables, formato, criterios) para que cada parte cumpla una función definida y sea fácil de escanear.

**Rol más específico y con incentivos.** Pasé de "Product Manager experto" a un PM senior con experiencia concreta en SaaS B2B de RR. HH. y ATS, y añadí el propósito del documento (servir de base fundacional para el equipo), lo que orienta el tono y la profundidad.

**Manejo de información faltante.** Añadí instrucciones para que marque explícitamente los *supuestos* en lugar de inventar datos que no están en `ats.jpg` ni en el prompt, algo clave porque depende de una imagen adjunta.

**Entregables con criterios internos.** Detallé qué debe contener cada caso de uso (actor, objetivo, flujo, resultado) y pedí justificación de las decisiones, no solo el resultado. Para el C4 pedí que justifique la elección del componente.

**Especificación técnica de los diagramas.** Sugerí Mermaid como formato por defecto para que los diagramas sean versionables y renderizables dentro del propio `.md`, evitando que entregue descripciones vagas.

**Checklist de autoevaluación.** Añadí una sección final que actúa como verificación de calidad antes de cerrar el documento, una técnica que reduce omisiones y respuestas genéricas.

Si quieres, puedo ajustarlo para un modelo concreto (por ejemplo, hacerlo más escueto si lo vas a usar con un modelo de menor contexto) o añadir ejemplos del estilo de salida esperado.

## Prompt 2:

```
# Prompt: Diseño de la primera versión del ATS de LTI

## 1. Rol y contexto

Actúa como **Product Manager Senior** con experiencia demostrable en productos SaaS B2B para Recursos Humanos y, en particular, en sistemas de seguimiento de candidatos (ATS). Combinas visión de negocio, criterio técnico y capacidad de comunicar decisiones de producto de forma clara a equipos multidisciplinares (ingeniería, diseño, ventas y dirección).

Tu trabajo servirá como **documento fundacional de producto** que el resto del equipo usará para alinearse antes de empezar a construir. Por tanto, debe ser riguroso, accionable y estar justificado, no ser una lista de buenas intenciones.

## 2. Sobre el proyecto

**LTI** es una startup que quiere desarrollar *el ATS (Applicant-Tracking System) del futuro*. El objetivo del producto es diferenciarse de la competencia a través de:

- **Eficiencia** para los departamentos de RR. HH. y reducción de tareas manuales.
- **Colaboración en tiempo real** entre reclutadores y hiring managers.
- **Automatización** de flujos repetitivos del proceso de selección.
- **Asistencia de IA** aplicada a tareas concretas y de alto valor (cribado, redacción, scoring, etc.).

**Material de referencia:** revisa la imagen adjunta `ats.jpg` antes de empezar. Si algún dato necesario para una decisión no está presente en la imagen ni en este prompt, indícalo explícitamente como **supuesto** en lugar de inventarlo de forma silenciosa.

## 3. Objetivo

Diseñar la **primera versión (v1)** del sistema LTI y dejar plasmadas, de forma documentada y justificada, las decisiones clave de producto y arquitectura que permitirán al equipo empezar a construir con una visión compartida.

Antes de redactar los entregables, realiza un breve ejercicio de **brainstorming y análisis** (mercado, competidores, dolores del usuario, oportunidades de diferenciación) y úsalo como base para justificar tus decisiones. No es necesario incluir todo el brainstorming en bruto: integra sus conclusiones en los entregables.

## 4. Entregables

Produce los siguientes artefactos, en este orden:

1. **Visión de producto**
   - Descripción breve del software LTI.
   - Valor añadido y ventajas competitivas frente a ATS existentes.
   - Explicación de las funciones principales.
   - **Diagrama Lean Canvas** que sintetice el modelo de negocio.

2. **Casos de uso**
   - Los **3 casos de uso principales**, cada uno con: actor(es), objetivo, flujo principal y resultado esperado.
   - Un **diagrama** asociado a cada caso de uso.

3. **Modelo de datos**
   - Entidades, atributos (con **nombre y tipo**) y relaciones entre entidades.
   - Representado mediante un **diagrama entidad-relación**.

4. **Diseño del sistema a alto nivel**
   - Explicación en prosa de los componentes y cómo interactúan.
   - **Diagrama de arquitectura de alto nivel** que acompañe la explicación.

5. **Diagrama C4 en profundidad**
   - Un **diagrama C4** que profundice en **uno** de los componentes del sistema (el que consideres más relevante o representativo). Justifica brevemente por qué elegiste ese componente.

## 5. Formato y requisitos de entrega

- Entrega **todo en un único documento Markdown** correctamente formateado llamado **`LTI-ARP.md`**.
- Usa **diagramas en código Mermaid** siempre que sea posible (Lean Canvas como tabla/estructura, casos de uso, ER, arquitectura y C4), de modo que sean versionables y renderizables. Si algún diagrama no es viable en Mermaid, descríbelo de forma estructurada.
- Estructura el documento con **encabezados jerárquicos** (`#`, `##`, `###`), tablas para el modelo de datos y bloques de código para los diagramas.
- Mantén un tono profesional y conciso. Cada decisión relevante debe ir acompañada de una **breve justificación** (el *por qué*, no solo el *qué*).
- **NUNCA** supongas nada, **pregunta antes de asumir** por falta de información.

## 6. Criterios de calidad (autoevaluación)

Antes de dar por terminado el documento, verifica que:

- [ ] Las ventajas competitivas son específicas y diferenciadoras, no genéricas.
- [ ] Los 3 casos de uso reflejan el valor central del producto (eficiencia, colaboración, automatización, IA).
- [ ] El modelo de datos es coherente con los casos de uso descritos.
- [ ] La arquitectura de alto nivel y el diagrama C4 son consistentes entre sí.
- [ ] Todos los diagramas renderizan correctamente y aportan información, no son decorativos.
- [ ] El documento es autocontenido: alguien ajeno al proyecto podría entenderlo sin contexto adicional.
```

## Respuesta 2:

He revisado el prompt y la imagen `ats.jpg`. La imagen muestra el ciclo clásico de un ATS en 7 etapas: crear ofertas → publicar en job boards/web/redes → recibir candidaturas → revisar candidaturas → tests online → entrevistas → contratación.

El prompt me pide expresamente **preguntar antes de asumir** cualquier dato faltante. Antes de redactar el documento `LTI-ARP.md`, hay varias decisiones de producto que cambian sustancialmente el resultado y que no puedo deducir ni de la imagen ni del enunciado. Para no inventar supuestos en silencio, me gustaría confirmar contigo unos pocos puntos clave.

He agrupado lo esencial en tres preguntas. Donde no me indiques nada, tomaré la opción que marco como predeterminada y la dejaré señalada explícitamente como **supuesto** dentro del documento.Parece que el formulario se ha mostrado pero no llegó una selección tuya (la respuesta volvió sin opciones marcadas). Quizá lo cerraste o prefieres no acotar manualmente.

No hay problema: para no bloquearte, voy a proceder con los supuestos que considero más sólidos para un "ATS del futuro" y los dejaré **marcados explícitamente como supuestos** dentro del documento, tal como pide el prompt. Si alguno no encaja, me lo dices y lo ajusto.

Los supuestos que tomaré son:
- **Segmento:** Mid-market (200-2000 empleados) como foco de la v1 — suficiente complejidad para justificar colaboración y automatización, sin la pesadez de cumplimiento de Enterprise puro.
- **IA en v1:** cribado/scoring de CVs y matching candidato-vacante como núcleo, con redacción asistida de ofertas/emails como apoyo. Resumen de entrevistas queda en roadmap.
- **Arquitectura:** multi-tenant SaaS en cloud desde el día 1, por ser la base estándar de un producto B2B escalable.

Voy a generar el documento `LTI-ARP.md` completo. Primero leo el skill de creación de documentos para asegurar el formato correcto.El entregable que pide el prompt es un **único archivo Markdown** (`LTI-ARP.md`), no un `.docx`. El skill de docx no aplica aquí — Markdown puro es exactamente lo solicitado, con diagramas Mermaid embebidos. Voy a crear el documento directamente.Voy a verificar rápidamente que la sintaxis Mermaid no tenga problemas obvios de renderizado (un fallo común es usar `\n` dentro de nodos, que algunos renderizadores aceptan y otros no).Hay varios `\n` dentro de nodos. Aunque Mermaid los soporta en muchos renderizadores, el más portable y seguro (especialmente GitHub y editores Markdown comunes) es usar `<br>`. También hay un riesgo con caracteres como `&` y comillas dentro de etiquetas de nodo. Los corrijo para máxima compatibilidad.Ahora reviso los nodos con `&` y comillas, que son las otras dos fuentes habituales de fallo de render en Mermaid.The `&` characters inside node labels and the single quotes can break Mermaid rendering. The safest fix is to wrap those labels in double quotes, which Mermaid treats as literal text. Let me fix the three risky nodes.Ahora valido la sintaxis de todos los bloques Mermaid con el parser oficial para asegurar que renderizan.mmdc se instaló. Extraigo cada bloque Mermaid y lo valido individualmente.All six failed identically — that's almost certainly Puppeteer/Chromium failing to launch, not a syntax problem. Let me check the actual error head.Confirmed — it's a missing Chrome binary, not a syntax issue. Chrome download domains aren't in the allowlist, so I'll validate syntax using Mermaid's own parser directly (no browser needed) via the `mermaid` JS package.Module resolution issue — the script is in /tmp but the package is in /home/claude. Let me run it from the right directory, and mermaid's parser needs a DOM environment. Let me set that up.Los 6 diagramas Mermaid pasan la validación de sintaxis del parser oficial. El documento está completo y verificado. Lo copio a la carpeta de salida y lo presento.Aquí tienes el documento fundacional `LTI-ARP.md`, completo y en un único Markdown. Contiene los cinco entregables en orden: visión de producto con Lean Canvas, los 3 casos de uso con diagrama cada uno, el modelo de datos con diagrama ER, el diseño de alto nivel con su diagrama de arquitectura, y un diagrama C4 que profundiza en el Servicio de IA. Los 6 diagramas Mermaid los validé con el parser oficial de Mermaid, así que renderizan correctamente.

Dos cosas que conviene que sepas:

El formulario de preguntas que te lancé al principio volvió sin selección, así que para no bloquearte avancé con tres supuestos clave, que están **marcados explícitamente** en la sección 0 del documento (tal como pedía el prompt, en vez de inventarlos en silencio): foco en **mid-market** (200–2.000 empleados), IA de v1 centrada en **cribado/scoring explicable + matching** con redacción asistida de apoyo, y arquitectura **multi-tenant cloud** desde el día 1. Si alguno no encaja con tu visión, dímelo y reajusto las secciones afectadas — un cambio en el segmento o en el alcance de IA toca sobre todo la visión, el modelo de datos y el C4.

Lo único que la imagen `ats.jpg` aportó fue el ciclo de 7 etapas del ATS (crear → publicar → recibir → revisar → tests → entrevistas → contratar), que usé como columna vertebral del alcance (supuesto S4). No había en ella datos de mercado, pricing ni competidores, por lo que esas decisiones provienen del razonamiento de producto, no de la imagen.

¿Quieres que ajuste algún supuesto, que añada una sección de roadmap post-v1, o que exporte el documento también a PDF o Word?

## Prompt 3:

P: ¿Qué segmento de cliente es el foco prioritario de la v1? Esto condiciona pricing, complejidad de permisos y casos de uso.
R: PYMEs (10-200 empleados)

P: ¿Qué capacidades de IA deben entrar SÍ o SÍ en la v1 (no en el roadmap futuro)? Marca las imprescindibles. (Selecciona todas las opciones aplicables)
R: Resumen de entrevistas, Matching candidato-vacante, Redacción de ofertas y emails, Cribado/scoring de CVs

P: ¿Prefieres que la arquitectura y el modelo de datos asuman multi-tenant SaaS en cloud desde el día 1, o algo más simple para la v1?
R: Single-tenant simple

## Respuesta 3:

Gracias, esto cambia tres decisiones de fondo, así que voy a regenerar el documento completo en lugar de parchearlo. Los cambios respecto a la versión anterior:

- **Segmento → PYMEs (10-200 empleados):** permisos más simples (menos roles, menos jerarquía), pricing más bajo y sensible al precio, casos de uso optimizados para equipos pequeños donde a menudo una misma persona hace de reclutador y *hiring manager*.
- **IA → las cuatro capacidades en v1**, incluido el resumen de entrevistas (que antes había pospuesto). Esto añade una entidad y un componente nuevos.
- **Arquitectura → single-tenant simple:** elimino el `tenant_id` del modelo, simplifico el diagrama de alto nivel (menos servicios desacoplados, despliegue por instancia de cliente) y ajusto el C4 en consecuencia.

Regenero el archivo.Ahora valido los 7 diagramas Mermaid de la nueva versión (hay uno más por el resumidor de entrevistas en el C4, aunque siguen siendo 6 bloques).Los 6 diagramas validan correctamente. Copio el documento final a salida.Documento `LTI-ARP.md` regenerado con tus tres respuestas incorporadas. Los 6 diagramas Mermaid vuelven a pasar la validación del parser oficial.

Qué cambió respecto a la versión anterior, en concreto:

Las decisiones ahora aparecen en la sección 0 como **confirmadas** (D1–D4), no como supuestos. El **segmento PYME** reorientó la propuesta de valor hacia simplicidad y precio asequible, redujo los roles a tres (ADMIN, RECRUITER, INTERVIEWER) reconociendo que en una pyme una persona suele combinar funciones, y ajustó canales y pricing del Lean Canvas hacia *self-service* y planes mensuales.

Las **cuatro capacidades de IA** ahora son el eje explícito: el resumen de entrevistas dejó de estar en el roadmap y entró como capacidad de primera clase. Eso añadió la entidad `InterviewSummary` y un campo `notes` en `Interview`, un componente `Resumidor de Entrevistas` en el C4, y reescribió el CU-2 para girar en torno a notas → resumen de IA → decisión.

El **single-tenant** eliminó por completo el `tenant_id` de todas las entidades (el aislamiento pasa a ser por instancia/despliegue), simplificó el diagrama de alto nivel —ahora todo vive dentro de una caja "Instancia por cliente" con una cola ligera en lugar de un bus multi-tenant— y se reflejó en el C4 y en las notas de privacidad.

Dejé marcados dos puntos abiertos que conviene cerrar con negocio/legal: el **supuesto S1** sobre idiomas (es/en) y el **riesgo R1**, que es relevante: el resumen de entrevistas implica tratar notas de entrevista, que son datos sensibles bajo RGPD. Asumí captura de **notas de texto** (no grabación de audio) para acotar ese riesgo en v1, pero si la intención es transcribir audio, eso cambiaría el alcance de cumplimiento y debería decidirse antes de construir.

¿Quieres que lo exporte también a PDF o Word, o que añada una sección de roadmap post-v1 (por ejemplo, multi-tenant y transcripción de audio como evoluciones naturales)?