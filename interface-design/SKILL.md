---
name: interface-design
description: Diseña, audita y corrige interfaces web y móviles interpretando la intención y el contexto del usuario. Aplica criterios de jerarquía visual, navegación, contenido, interacción y decisiones de producto a pantallas, componentes y flujos; no se limita a palabras clave ni a frases de activación.
---

# Interface Design

Convierte la intención del usuario en una interfaz comprensible y utilizable o en un diagnóstico accionable. Responde en su idioma. Usa las reglas como criterios de decisión contextual, no como una estética predeterminada.

## Interpretar el encargo

Determina el resultado esperado a partir del significado completo de la conversación, los artefactos disponibles y las restricciones. No uses un clasificador de palabras clave ni exijas que el usuario nombre un modo.

- Si necesita una interfaz inexistente o una nueva capacidad, crea el diseño correspondiente.
- Si busca comprender la calidad, las causas de un problema o las oportunidades, audita y entrega conclusiones sin modificar el producto.
- Si pide mejorar o resolver problemas de una interfaz existente, diagnostica lo necesario, corrige dentro del alcance y verifica. No te detengas en un informe cuando pidió cambios.
- Combina estos trabajos cuando la intención lo requiera. Un comentario de insatisfacción por sí solo no siempre autoriza cambios: interpreta si pide explicación, alternativas o ejecución.

Considera plataforma, tarea principal, usuarios, identidad existente, alcance, estados y restricciones técnicas. Inspecciona el material que exista antes de suponer cómo funciona o se ve el producto. Pregunta solo por ambigüedades que cambien materialmente el resultado; avanza en lo independiente. No amplíes un ajuste local a un rediseño completo.

## Criterios compartidos

Lee [design-principles.md](references/design-principles.md) al diseñar o evaluar una interfaz. Aplica únicamente los criterios relevantes. Conserva los tokens, componentes e identidad del producto salvo que el encargo pida cambiarlos.

Prioriza comprensión, finalización de la tarea, legibilidad y recuperación sobre decoración. Distingue un defecto observable de una preferencia estética o una hipótesis que necesita datos. No atribuyas aumentos de conversión a cambios no medidos.

Los principios proceden de transcripciones aportadas por el usuario; consulta [video-sources.md](references/video-sources.md) cuando necesites explicar su origen o sus límites. No afirmes haber visto los ejemplos visuales originales.

## Crear

1. Identifica la tarea principal y las decisiones que deben permanecer juntas. Define la estructura, la navegación y la acción principal antes de pulir estilos.
2. Diseña con contenido representativo: nombres largos, imágenes variables y cantidades plausibles. Identifica datos simulados; no inventes reseñas, disponibilidad o personalización como hechos.
3. Desarrolla los componentes y estados pertinentes al alcance: inicial, vacío, sin resultados, carga, error, selección y éxito cuando correspondan.
4. Implementa si eso forma parte del encargo, reutilizando el proyecto. Si se pidió solo diseño, entrega el artefacto de diseño solicitado.
5. Verifica con los criterios de [audit-criteria.md](references/audit-criteria.md), limitando la revisión al trabajo realizado y sus efectos.

## Auditar

Lee [audit-criteria.md](references/audit-criteria.md). Examina la interfaz y el flujo con las herramientas disponibles. Una captura permite evaluar su estado visible, no confirmar comportamiento, accesibilidad completa o adaptación a otros tamaños.

Entrega hallazgos priorizados con ubicación, evidencia, impacto, corrección y forma de verificar. No llenes una cuota de problemas ni uses puntuaciones arbitrarias. Señala qué no pudo comprobarse. No cambies archivos del producto cuando el encargo sea únicamente una revisión.

## Corregir

Obtén evidencia suficiente, prioriza los problemas que bloquean la tarea y aplica cambios proporcionales. Evita imponer un nuevo lenguaje visual para resolver defectos de espaciado o jerarquía. Comprueba los estados afectados y compara el resultado con la referencia disponible. Resume qué cambió, por qué, qué se verificó y las limitaciones restantes.

## Colaboración con otras skills

Esta skill es autónoma: no requiere Impeccable, Mobbin ni preview-components. Si el usuario solicita alternativas y aplica `preview-components`, usa estos criterios para fundamentar sus propuestas y respeta su flujo de elección antes de implementar. No conviertas las tres alternativas en un requisito para toda creación, auditoría o corrección. No invoques otras skills por compartir únicamente palabras como «diseño».
