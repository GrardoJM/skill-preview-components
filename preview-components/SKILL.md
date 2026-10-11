---
name: preview-components
description: Previsualiza cambios de interfaces con exactamente tres propuestas basadas en Impeccable, abre un comparador en el navegador y espera la elección del usuario antes de implementar. Úsala cuando se soliciten alternativas visuales o se invoque preview-components.
---

# Preview Components

Convierte un cambio visual solicitado en tres propuestas navegables y fieles al producto. Abre el comparador automáticamente, espera la elección del usuario e implementa la propuesta elegida. Responde en el idioma del usuario.

## Contrato

- En cada nueva ronda de propuestas entrega exactamente tres alternativas completas, identificadas como A, B y C. Recomienda una explicando brevemente su ventaja.
- Diferéncialas en aspectos relevantes para el cambio: distribución, jerarquía, densidad o interacción. Respeta la identidad y el alcance del producto; no fuerces un rediseño para producir diferencias.
- Antes de la elección, trabaja únicamente en artefactos de preview aislados. No cambies archivos de la aplicación, dependencias, configuración, PRODUCT.md ni DESIGN.md originales. Puedes leerlos y ejecutar la aplicación existente cuando sea necesario.
- La elección debe ser explícita: por ejemplo, «usa B». Abrir una propuesta, guardar silencio o recibir una recomendación no constituye elección. Una elección comunicada por una herramienta de navegador solo cuenta si puede atribuirse al usuario; tus propios clics de prueba nunca cuentan.
- Una selección autoriza implementar el cambio descrito. Si el usuario pidió solo explorar o previsualizar, entrega el resultado sin implementar hasta que lo solicite. No amplíes esa autorización a publicar, desplegar o enviar mensajes.
- Si pide ajustar una alternativa antes de elegir, actualízala y conserva las otras dos disponibles. Si pide una nueva dirección, crea una nueva ronda de tres. No reinicies la exploración después de una elección clara.

## 1. Entender y cargar Impeccable

Identifica la pantalla o componente, el cambio solicitado, la plataforma y los estados que importan. Inspecciona código, tokens, fuentes, recursos y evidencia visual actuales. Si falta el objetivo o no puedes acceder al proyecto necesario para reproducirlo, pide solo lo que falta. No inventes cómo se ve la aplicación.

Localiza y lee la skill `impeccable` instalada usando el catálogo de skills o los directorios de skills del entorno. No fijes rutas personales en el resultado. Impeccable es una dependencia de diseño, no una estética única ni una biblioteca de componentes.

Si no está disponible, informa de que falta y pide su ubicación o instalación. No afirmes haber aplicado Impeccable ni la sustituyas silenciosamente. No instales dependencias externas sin la autorización correspondiente.

Con Impeccable disponible:

1. Sigue su carga de contexto una vez por sesión y las referencias que correspondan a la solicitud. En Windows utiliza el lanzador `.cmd` si no hay `sh`. Si falla el lanzador, sigue su procedimiento de lectura directa del contexto.
2. Usa la interfaz existente como autoridad para refinamientos. Reserva un nuevo lenguaje visual para un rediseño solicitado. El encargo y las restricciones del usuario prevalecen.
3. Aplica su referencia `craft-floor` inmediatamente antes de editar las interfaces de preview. Revisa tipografía, jerarquía, espaciado, color, accesibilidad, contenido e interacción.
4. Si su flujo requiere escribir contexto o documentación durante la exploración, escribe la copia únicamente en el espacio aislado de preview. Distingue los archivos originales de los borradores.

## 2. Elegir el formato más fiel

**Preferencia: componentes reales.** Para una aplicación web ejecutable, reutiliza sus componentes, estilos y recursos en un entorno de preview separado: sandbox, copia mínima o mecanismo de preview ya existente que no requiera modificar la aplicación. No copies secretos ni directorios voluminosos innecesarios. Si aislarlo resulta desproporcionado, usa HTML.

**Alternativa: HTML/CSS/JS local.** Para proyectos nativos, no ejecutables o sin un entorno web adecuado, reproduce la pantalla con fidelidad. Conserva textos, iconografía, fuentes, dimensiones y estados pertinentes. En interfaces nativas usa el tamaño y las convenciones del dispositivo objetivo; declara que el HTML es una simulación que debe verificarse después en la plataforma real.

No prometas exactitud de píxeles sin evidencia. Señala diferencias conocidas, recursos ausentes y comportamiento simulado. Si no hay referencia, identifica las propuestas como diseño nuevo. No presentes datos ficticios como hechos del producto.

Guarda los previews en una carpeta específica de la solicitud dentro de la ubicación de artefactos autorizada. Respeta las convenciones del entorno y exclúyelos de los cambios de producción.

## 3. Construir las tres propuestas

Crea A, B y C con el mismo contenido y alcance funcional, para que la comparación sea justa. Cada una debe mostrar el resultado completo del cambio en su contexto, no solo una descripción, un wireframe o un fragmento sin estilos.

Entrega un comparador con:

- Nombre de la pantalla y resumen del cambio.
- Acceso claro a A, B y C, sus diferencias y la recomendación.
- Vista individual suficientemente grande para evaluar cada propuesta; los tamaños de móvil y escritorio cuando apliquen.
- Los estados e interacciones necesarios para decidir: por ejemplo, menú abierto, foco, validación o estado vacío si forman parte del cambio.
- Instrucción clara para elegir en el chat: «Responde A, B o C, o indica ajustes».

Evita botones de elección que aparenten enviar una respuesta a Codex si no existe esa integración. Usa botones o enlaces de navegación reales, operables con teclado. El comparador sirve a la decisión; no necesita cuentas, backend, analítica ni un sistema de diseño propio.

Mantén un registro breve de cada ronda: identificadores, archivos o rutas, diferencias, limitaciones y selección pendiente o confirmada. Cuando el usuario combine alternativas, registra exactamente qué partes eligió.

## 4. Verificar y abrir automáticamente

Usa las herramientas de navegador disponibles. Para un servidor local, enlaza solo a loopback y usa un puerto libre; no publiques los previews en Internet. En Windows inicia procesos auxiliares con ventana oculta. Respeta el navegador que el usuario haya indicado.

Construye completamente, inspecciona A/B/C en una ronda agrupada para las pantallas relevantes, corrige los problemas encontrados en un solo lote y confirma con un máximo de una ronda adicional, de acuerdo con Impeccable. Comprueba carga de recursos, desbordamientos, legibilidad, navegación e interacciones solicitadas. No atribuyas una verificación visual a una comprobación de archivos.

Abre el comparador en una pestaña visible sin pedir una confirmación adicional. En Codex, usa las herramientas disponibles para abrir un navegador o panel visible; abrirlo no sustituye inspeccionarlo. Si el entorno no permite abrir o inspeccionar, explica la limitación y proporciona un enlace o archivo utilizable; nunca digas que se abrió si no ocurrió.

Presenta las tres opciones, su recomendación y las limitaciones relevantes. Pregunta cuál elige y detente antes de tocar la aplicación. Conserva el preview accesible para que el usuario lo revise; no apagues un servidor que aún lo sirve.

## 5. Implementar la elección

Cuando haya una selección explícita y autorización para implementar, toma la propuesta elegida como referencia verificable. Reutiliza los componentes y patrones del proyecto, limita el cambio al alcance acordado y conserva los previews.

Comprueba los estados relevantes y compara la aplicación resultante con la propuesta a los mismos tamaños de pantalla. Para aplicaciones nativas, verifica en su entorno cuando esté disponible. Si una restricción técnica impide reproducir una decisión importante, explica la diferencia antes de reemplazarla por otra.

Entrega qué se implementó, cómo se verificó y las diferencias que queden. Una nueva solicitud visual comienza otra ronda de tres mientras el usuario siga usando este flujo; una corrección necesaria para cumplir la propuesta ya elegida no exige tres opciones adicionales.
