# Laboratorio adicional 5

Realiza pruebas de rendimiento sobre la funcionalidad de reserva de pasajes en [blazedemo](https://www.blazedemo.com/) utilizando JMeter.

## Instrucciones

1. **Generar el archivo .jmx:**  
   Crea un plan de pruebas en JMeter que incluya las acciones necesarias para simular la reserva de pasajes en el sitio. Guarda el plan como archivo `.jmx`.

2. **Configurar escenarios de usuarios:**  
   - Ajusta el número de hilos (usuarios) en el plan de pruebas: primero configura 1 usuario y luego 50 usuarios concurrentes.
   - Incorpora al menos dos listeners (por ejemplo, "View Results Tree" y "Summary Report") para visualizar y analizar los resultados.
   - Añade al menos una assertion para validar que la respuesta del servidor sea correcta (por ejemplo, comprobando el código de estado HTTP o la presencia de un texto específico en la respuesta).

3. **Ejecutar y analizar las pruebas:**  
   - Ejecuta las pruebas en ambos escenarios (1 y 50 usuarios).
   - Observa y compara los resultados obtenidos en los listeners, prestando atención a los tiempos de respuesta, tasas de error y cualquier incidencia detectada por las assertions.
   - Documenta tus observaciones y conclusiones sobre el comportamiento de la funcionalidad bajo diferentes cargas.

> **Recomendación:** Puedes consultar la [documentación oficial de JMeter](https://jmeter.apache.org/usermanual/index.html) para detalles sobre la configuración de listeners y assertions.

---

[⬅️ Volver al índice del módulo](../modulo5_pruebas_no_funcionales.md)  
[🏠 Menú principal](../README.md)