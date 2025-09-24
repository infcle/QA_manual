# Laboratorio adicional 2 resuelto

## Solución del ejercicio 1

- **Conceptos básicos**  
Las pruebas de carga son un tipo de pruebas no funcionales de rendimiento que simulan la interacción de múltiples usuarios con un sistema o servicio web de manera simultánea. Su objetivo es evaluar los tiempos de respuesta, la latencia y la cantidad de datos enviados y recibidos, verificando que el sistema funcione correctamente bajo una carga esperada según la infraestructura disponible.

- **Beneficios y desventajas**  
*Beneficios:*  
a) Permiten simular el comportamiento del sistema bajo alta demanda, proporcionando información valiosa para tomar decisiones sobre desarrollo e infraestructura.  
b) Ayudan a identificar cuellos de botella en transacciones o funcionalidades que pueden ralentizar el sistema.

*Desventajas:*  
a) Puede ser difícil definir con precisión el número de usuarios que el sistema debe soportar.  
b) Es complicado replicar el entorno de producción, y a veces no se dispone de ambientes dedicados para ejecutar pruebas de carga.  
c) Los resultados pueden variar según el momento de ejecución y el equipo cliente utilizado.

- **Elementos o dispositivos en los que aplica**  
a) La conectividad y capacidad del servidor donde opera el sistema.  
b) Recursos como memoria y disco del servidor.  
c) El propio sistema, ya que se pueden detectar funcionalidades que consumen más recursos de lo esperado, lo que representa oportunidades de optimización.

- **Herramientas de monitoreo que pueden colaborar**  
Para evaluar el rendimiento de una aplicación se pueden utilizar:  
a) Herramientas de monitoreo de velocidad, que permiten analizar la carga inicial de un sitio web y extraer métricas como tiempos de carga, bloqueos antes del primer uso y cantidad de peticiones involucradas.  
b) Herramientas de pruebas de rendimiento, que simulan múltiples usuarios (hilos de ejecución) utilizando el sistema simultáneamente para generar estadísticas y métricas sobre tiempos de respuesta y realizar comprobaciones adicionales.

---

[⬅️ Volver al índice del módulo](../modulo5_pruebas_no_funcionales.md)  
[🏠 Menú principal](../README.md)
