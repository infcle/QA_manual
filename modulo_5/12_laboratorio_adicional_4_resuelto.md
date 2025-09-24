# Laboratorio adicional 4 resuelto

## Solución del ejercicio 1

A continuación se describe el contenido típico de un plan de pruebas no funcionales, utilizando un ejemplo práctico:

- **Motivo:**  
Explica la razón por la cual se requieren pruebas de rendimiento.  
*Ejemplo:* Durante la última temporada de descuentos, el sistema e-commerce ABC presentó caídas al alcanzar 200 usuarios concurrentes. Por ello, se solicita ejecutar pruebas de rendimiento para identificar los incidentes y aplicar medidas correctivas que permitan soportar al menos 500 usuarios concurrentes.

- **Pasos de ejecución:**  
Enumera las acciones y escenarios que se llevarán a cabo durante las pruebas.  
*Ejemplo:* Se planifica ejecutar pruebas de rendimiento en el sistema e-commerce ABC bajo diferentes cargas: 1, 50, 100, 300 y 500 usuarios concurrentes, simulando transacciones de compra, navegación y pago.

- **Pre-requisitos:**  
Detalla los recursos y condiciones necesarias antes de iniciar las pruebas.  
*Ejemplo:* Se requiere un ambiente dedicado con características similares al entorno de producción, acceso a la base de datos, conectividad estable y un servidor cliente para lanzar los hilos de ejecución.

- **Herramientas y código fuente:**  
Indica las herramientas y utilidades que se emplearán para ejecutar y analizar las pruebas.  
*Ejemplo:* Se utilizará Apache JMeter versión 5.4.1 para la simulación de usuarios y la recolección de métricas. El código fuente de los scripts de prueba estará disponible en el repositorio del proyecto.

- **Criterios de paso o fallo:**  
Define las condiciones que determinan el éxito o fracaso de las pruebas.  
*Ejemplo:* Las pruebas serán exitosas si todos los escenarios se ejecutan sin defectos críticos y el sistema mantiene tiempos de respuesta aceptables. Se considerará fallo si se detecta un defecto bloqueante, como la caída del servidor al superar los 100 usuarios concurrentes.

- **Rango de carga:**  
Especifica los niveles de carga que se utilizarán en las pruebas.  
*Ejemplo:* Se simularán cargas de 1, 50, 100, 200 y 500 usuarios concurrentes para evaluar el comportamiento del sistema en distintos escenarios.

- **Datos a recolectar:**  
Establece las métricas e indicadores que se recopilarán durante las pruebas.  
*Ejemplo:* Tiempo de respuesta por transacción, bytes enviados y recibidos, porcentaje de transacciones con error, uso de CPU y memoria, y disponibilidad del sistema.

---

## Solución del ejercicio 2

Pasos necesarios para elaborar un plan de pruebas no funcionales:

1. **Conocer los ambientes a testear:**  
Identificar los entornos donde se ejecutarán las pruebas (desarrollo, pre-producción, producción) y sus características técnicas.

2. **Definir los criterios de aceptación:**  
Establecer los parámetros que determinarán si el sistema cumple con los requisitos de rendimiento, seguridad, escalabilidad, etc.

3. **Elaborar el plan de pruebas:**  
Documentar el alcance, objetivos, recursos, cronograma y responsables de las pruebas no funcionales.

4. **Diseñar los casos de prueba:**  
Crear escenarios detallados que permitan evaluar el comportamiento del sistema bajo diferentes condiciones y cargas.

5. **Configurar el ambiente de pruebas:**  
Preparar la infraestructura, instalar las herramientas necesarias y asegurar que el entorno esté listo para la ejecución.

6. **Ejecutar las pruebas:**  
Realizar las pruebas siguiendo los casos diseñados, registrando los resultados y observaciones.

7. **Analizar resultados, generar reportes y realizar re-pruebas:**  
Interpretar los datos obtenidos, elaborar informes de resultados y, si es necesario, repetir las pruebas tras aplicar correcciones.

---

[⬅️ Volver al índice del módulo](../modulo5_pruebas_no_funcionales.md)  
[🏠 Menú principal](../README.md)
