# Principios de diseño contextual

Las referencias V1, V2 y V3 se resuelven en video-sources.md. Las precauciones de accesibilidad y verificación son adaptaciones operativas, no citas de los videos.

## Jerarquía, legibilidad y coherencia

- **Orden de lectura (V1, V3):** define qué debe reconocerse primero y qué sostiene la decisión. Usa tamaño, peso, espacio y color en conjunto; evita que todo compita. Verifica si se distinguen identidad, datos relevantes y acción al escanear.
- **Estructura y proximidad (V1):** alinea contenido sobre márgenes consistentes y acerca elementos relacionados. El espacio excesivo puede romper una relación tanto como el amontonamiento. No fijes 24 px como margen obligatorio.
- **Tipografía (V1, V2):** conserva tamaños cómodos en móvil; no reduzcas todo para encajar un escritorio. Una familia suele bastar, pero no prohíbas sistemas tipográficos justificados. Ajusta interlineado y etiquetas pequeñas sin degradar legibilidad. Las medidas mencionadas por los autores no sustituyen las unidades y convenciones de la plataforma.
- **Color e iconos (V1, V3):** reserva énfasis para información importante; usa estilos de iconos y geometría compatibles. Colores suaves, esquinas redondeadas o una fuente concreta no son requisitos universales. Usa separadores que organicen sin dominar.
- **Contenido breve (V1):** elimina redundancias en badges y etiquetas cuando el contexto siga siendo inequívoco. Quitar una etiqueta visual no justifica eliminar el nombre accesible de un control.
- **Contraste robusto (V1, V3):** los controles y textos deben funcionar con imágenes claras, oscuras y ocupadas. Usa contenedores, fondos o separación de la fotografía. Rebajar el protagonismo del texto secundario no debe volverlo ilegible. No certifiques accesibilidad sin mediciones y comprobaciones pertinentes.

## Imágenes y listados

- **Función de la imagen (V1, V3):** decide si sirve para identificar, comparar o despertar interés y dimensiona en consecuencia. No comprimas el contenido solo para mostrar más elementos antes del primer desplazamiento.
- **Sistema de catálogo (V1):** mantén foco en el producto y coherencia de encuadre, iluminación y tratamiento entre imágenes. Representa fielmente lo vendido; el ejemplo de fondo limpio para fruta no obliga a eliminar fotografía editorial en otros productos.
- **Competencia visual (V3):** reduce imágenes decorativas que compitan con las principales. Mantén detalles críticos fuera de fondos impredecibles si no puedes garantizar lectura.
- **Explorar o comparar (V3):** considera vistas alternativas cuando resuelvan necesidades reales diferentes. No añadas un selector de vista por defecto a todos los listados.

## Navegación y móvil

- **Prioridad en pantallas pequeñas (V2):** adapta estructura y tareas en lugar de encoger el escritorio. Una dirección principal de lectura por sección suele simplificar; una cuadrícula móvil puede ser válida si su contenido sigue siendo legible.
- **Destinos principales (V2):** una barra inferior funciona para pocos destinos; tres o cuatro son ejemplos preferidos del autor, cinco su límite orientativo. Si no encajan, reconsidera la arquitectura. No ocultes una función crítica sin una vía descubrible.
- **Agrupación (V2):** evita tarjetas anidadas que consumen el espacio con padding acumulado. Usa proximidad o encabezados cuando un contenedor adicional no aporta significado.
- **Tarea y contexto (V2, V3):** concentra cada pantalla en un propósito; conserva juntas las decisiones interdependientes. Usa un panel inferior para tareas auxiliares si mantiene el contexto y cabe adecuadamente. No fragmentes filtros relacionados solo para cumplir «una tarea por pantalla».
- **Acciones contextuales (V2):** muestra herramientas pertinentes al estado actual sin hacer impredecible la navegación principal. Los gestos deben ser descubribles y las acciones esenciales tener una alternativa accesible; no copies gestos de otra plataforma sin comprobar convenciones.
- **Movimiento (V2):** comunica continuidad y relación entre vistas. Los porcentajes, zooms y desenfoques del ejemplo no son valores obligatorios; considera preferencias de movimiento reducido y alternativas sin animación.
- **Estados vacíos (V2):** diferencia primer uso de ausencia de resultados. El primero orienta a comenzar; el segundo explica la búsqueda y ofrece ajustar, limpiar o salir. Evita imágenes decorativas que desplacen la salida útil.

## Producto y compra

- **Información oportuna (V1):** acerca identidad, valoración y precio cuando sostengan la decisión de compra. No inventes prueba social.
- **Cantidad inequívoca (V1):** distingue producto, unidad de venta, cantidad y total. No borres el tamaño de un paquete fijo solo porque exista selector de unidades; corrige únicamente la ambigüedad real.
- **Acción agrupada (V1):** relaciona selector y compra, muestra el coste resultante cuando sea útil y evita énfasis agresivo innecesario. Comprueba que el total se actualice al cambiar cantidades.
- **Persistencia útil (V1):** considera acción fija y contexto visible durante el scroll en flujos largos. Verifica que no tapen contenido, foco, teclado o áreas seguras. Una tarjeta superpuesta es una opción del ejemplo, no una plantilla universal.
- **Atajos con fundamento (V1):** ofrece cantidades frecuentes si existe evidencia o márcalas como hipótesis. Conserva flexibilidad cuando se necesiten valores diferentes.

## Búsqueda y filtros

- **Descubribilidad (V3):** muestra filtros frecuentes y acceso a los restantes; explica qué puede buscarse. Un placeholder no sustituye por sí solo una etiqueta accesible.
- **Decisiones relacionadas (V3):** permite comparar presupuesto, características y resultados sin navegar continuamente entre páginas aisladas.
- **Control adecuado (V3):** combina slider para explorar con entrada precisa cuando sea útil. Usa opciones directas para valores conocidos; steppers para ajustes incrementales.
- **Semántica explícita (V3):** distingue valor exacto, mínimo y rango. La selección de extremos de un rango necesita feedback claro; no supongas que el gesto se entiende por sí solo.
- **Consecuencias visibles (V3):** muestra resultados previstos o conteos por opción cuando el sistema pueda obtenerlos. Distingue carga, cero resultados y error; evita mostrar conteos antiguos como actuales.
- **Distribución y contexto (V3):** un histograma ayuda si explica opciones reales y sus trade-offs. Identifica a qué conjunto de datos corresponde y cómo cambian las cifras con los filtros.
- **Necesidades a parámetros (V3):** puede ser útil traducir un objetivo del usuario a valores de búsqueda. En estimaciones, expón supuestos y límites; no presentes un cálculo aproximado como garantía.
- **Complejidad justificada (V3):** personalización, vistas alternativas y datos adicionales deben ayudar a decidir. Una interfaz más compleja no es automáticamente más experta; usa divulgación progresiva si corresponde.
