# Mobile-Tests-for-Urban-Lunch 🥙 🍱  
Proyecto 5

## Introducción

El presente documento detalla los resultados de las pruebas realizadas a la aplicación móvil Urban.Lunch, un sistema de pedidos y entrega de alimentos. Las pruebas fueron ejecutadas en un entorno controlado utilizando Android Studio, específicamente con el emulador virtual Honor 8 API 28 (emulador-5554).

<a href="https://docs.google.com/spreadsheets/d/1IC8u2R1w2LvyjZCSHTf3DapvSNlUKBj_/edit?usp=sharing&ouid=103258639782325772763&rtpof=true&sd=true" target="_blank">
 📊​ Archivo original 
</a>

### Entorno de Pruebas

**Especificaciones Técnicas:**
- **IDE:** Android Studio
- **Dispositivo Virtual:**
  - Modelo: Honor 8
  - API Level: 28 (Android 9.0 Pie)
  - AVD Manager ID: emulador-5554
  - Resolución: 1080 x 1920 pixels
  - Densidad: 480dpi
  - RAM: 2GB

### Alcance de las Pruebas

Las pruebas abarcaron seis áreas funcionales principales:
1. Sistema de geolocalización y selección de puntos de recogida
2. Gestión de menú y selección de platillos
3. Proceso de pedido y confirmación
4. Sistema de seguimiento en tiempo real
5. Proceso de entrega y feedback
6. Manejo de errores y validaciones

### Metodología de Testing

1. **Pruebas Funcionales**
   - Validación de flujos principales
   - Pruebas de interfaz de usuario
   - Verificación de respuesta táctil
   - Pruebas de geolocalización

2. **Pruebas de Usabilidad**
   - Navegación entre pantallas
   - Accesibilidad de elementos
   - Claridad de información
   - Experiencia de usuario

3. **Pruebas de Integración**
   - Conexión con servicios de mapas
   - Integración con sistema de pagos
   - Sincronización de datos
   - Actualización en tiempo real

### Métricas Clave

- Total de casos de prueba: 60
- Casos exitosos: 45 (75%)
- Casos fallidos: 15 (25%)
- Bugs críticos identificados: 15
- Áreas con mayor incidencia: 
  - Geolocalización
  - Cálculo de tiempos
  - Manejo de errores

### Hallazgos Significativos

1. **Problemas Críticos**:
   - Fallos en la visualización de mapas y ubicaciones
   - Inconsistencias en cálculos de tiempo y costos
   - Errores en transiciones de estado de pedidos
   - Problemas con notificaciones y alertas

2. **Áreas de Mejora**:
   - Optimización de rendimiento en mapas
   - Mejora en la precisión de cálculos
   - Refinamiento de interfaces de usuario
   - Robustez en manejo de errores

3. **Impacto en Usuario Final**:
   - Experiencia interrumpida en seguimiento de pedidos
   - Confusión en costos y tiempos
   - Problemas de orientación en mapas
   - Inconsistencias en feedback


## Resumen de Resultados
| Categoría | Total | PASSED | FAILED | % Éxito |
|-----------|-------|--------|---------|---------|
| Total de Pruebas | 60 | 45 | 15 | 75% |

## Desglose por Funcionalidad

### 1. Selección punto de recogida
| ID | Descripción | Estado | Bug ID |
|----|-------------|--------|---------|
| 1 | Visualización de puntos de recogida y ubicación | FAILED | PLM1G5S-1 |
| 2 | Selección manual de puntos de recogida | PASSED | - |
| 3 | Listado de puntos en pie de página | FAILED | PLM1G5S-2 |
| 4 | Indicador visual de selección | PASSED | - |
| 5 | Actualización de punto seleccionado | PASSED | - |
| 6 | Cancelación de selección | PASSED | - |

### 2. Elección de platillos
| ID | Descripción | Estado | Bug ID |
|----|-------------|--------|---------|
| 7 | Visualización de nombres de platillos | PASSED | - |
| 8 | Botón de agregar (+) | PASSED | - |
| 9 | Botón de quitar (-) | PASSED | - |
| 10 | Validación de negativos | PASSED | - |
| 11 | Contador de platillos | PASSED | - |
| 12 | Botón de continuar | PASSED | - |
| 13 | Navegación a realizar pedido | PASSED | - |
| 14 | Asignación a restaurante cercano | PASSED | - |
| 15-18 | Funcionalidades de progreso y navegación | PASSED | - |

### 3. Detalles del platillo
| ID | Descripción | Estado | Bug ID |
|----|-------------|--------|---------|
| 19-22 | Información del platillo | PASSED | - |
| 23 | Interacción con nombre de restaurante | FAILED | PLM1G5S-3 |
| 24 | Interacción con costo | FAILED | PLM1G5S-4 |
| 25 | Interacción con tiempo de preparación | FAILED | PLM1G5S-5 |
| 26-27 | Navegación y agregar platillo | PASSED | - |
| 28 | Cálculo de tiempo de espera | FAILED | PLM1G5S-6 |
| 29-30 | Validaciones de pedido | PASSED | - |

### 4. Confirmar el pedido
| ID | Descripción | Estado | Bug ID |
|----|-------------|--------|---------|
| 31-36 | Información de pedido | PASSED | - |
| 37 | Cálculo de importe total | FAILED | PLM1G5S-7 |
| 38-42 | Progreso y confirmación | PASSED | - |

### 5. Seguimiento de pedidos
| ID | Descripción | Estado | Bug ID |
|----|-------------|--------|---------|
| 43 | Visualización punto de recogida | PASSED | - |
| 44 | Visualización restaurantes | FAILED | PLM1G5S-8 |
| 45 | Visualización de ruta | PASSED | - |
| 46 | Visualización de costos | FAILED | PLM1G5S-9 |
| 47 | Tiempo de preparación | FAILED | PLM1G5S-10 |
| 48-51 | Funcionalidades de seguimiento | PASSED | - |
| 52 | Transición a pedido listo | FAILED | PLM1G5S-11 |

### 6. Entrega y Feedback
| ID | Descripción | Estado | Bug ID |
|----|-------------|--------|---------|
| 53 | Transición a pedido entregado | FAILED | PLM1G5S-12 |
| 54-55 | Confirmación de entrega | PASSED | - |
| 56 | Navegación a feedback | FAILED | PLM1G5S-13 |
| 57-58 | Proceso de feedback | PASSED | - |

### 7. Manejo de Errores
| ID | Descripción | Estado | Bug ID |
|----|-------------|--------|---------|
| 59 | Error de geolocalización | FAILED | PLM1G5S-14 |
| 60 | Validación de pedido vacío | FAILED | PLM1G5S-15 |

## Observaciones Críticas
1. Problemas significativos en el manejo de errores
2. Inconsistencias en cálculos de tiempo y costos
3. Fallas en transiciones de estados de pedido
4. Problemas de visualización en mapas
5. Errores en la validación de interacciones

### Conclusión Preliminar

La aplicación muestra un funcionamiento base aceptable pero requiere correcciones significativas antes de su lanzamiento a producción. Los problemas identificados, especialmente en áreas críticas como geolocalización y cálculos de tiempo/costo, podrían impactar negativamente la experiencia del usuario y la confiabilidad del servicio.

