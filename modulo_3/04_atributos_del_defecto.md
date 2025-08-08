# Atributos del Defecto

## Contenido

- Atributos de un bug  
- Planilla de registro de bugs  
- Seguimiento de bugs  
- Ejercicio práctico de registración  

---

## Atributos de un Bug

- **ID:** Identificador único.  
- **Descripción:** Título breve del bug.  
- **Datos:** Información necesaria para ejecutar el caso de prueba y reproducir el bug.  
- **Tipo:** Tipo de defecto (software, datos, ambiente, interconexión, etc.).  
- **Prioridad:** Importancia de la corrección del bug.  
- **Severidad:** Grado de impacto en el negocio.  
- **Ciclo:** Etapa del ciclo de pruebas en la que fue detectado.  
- **Estado (Status):** Abierto, en proceso, asignado, resuelto, cerrado o anulado.  
- **Tester:** Responsable que detectó el defecto.  
- **Evidencia:** Captura de pantalla, archivo o foto que demuestra el bug.  
- **Asignado a:** Desarrollador responsable de resolver el bug.  

---

## Planilla de Bugs

| Atributo               | Descripción |
|------------------------|-------------|
| **ID Bug**             | Identificador mnemotécnico del bug |
| **ID Sistema**         | Identificador mnemotécnico del sistema |
| **ID CU**              | Nombre mnemotécnico del caso de uso |
| **ID CP**              | Nombre mnemotécnico del caso de prueba |
| **ID Paso**            | Número de paso del caso de prueba |
| **Título**             | Breve resumen o nombre mnemotécnico del bug |
| **Descripción**        | Explicación detallada para reproducir y resolver el bug |
| **Estado (Status)**    | Abierto, asignado, resuelto, cerrado, etc. |
| **Prioridad**          | Urgencia/importancia de la corrección (Alta, Media, Baja) |
| **Severidad**          | Alcance o impacto en el negocio |
| **Ciclo**              | Ciclo de ejecución de pruebas según la estrategia |
| **Evidencia (link)**   | Captura de pantalla, archivo, XML, etc. |
| **Responsable Tester** | Nombre del tester que detectó el bug |
| **Fecha detectada**    | Día en que se registró el defecto |
| **Fecha estimada de entrega** | Fecha prevista para la corrección |
| **Área asignada**      | Área responsable de la resolución |
| **Descripción de resolución** | Explicación de cómo se resolvió |
| **Fecha real de entrega** | Fecha efectiva de entrega de la corrección |
| **Fecha de cierre**    | Día en que se cerró el bug |

---

## Seguimiento de Bugs

1. Revisar el **backlog** de defectos asignados.  
2. Utilizar el **módulo de defectos** de la herramienta de gestión.  
3. Aplicar **filtros** para revisar únicamente los defectos asignados.  
4. **Reprobar** los defectos que figuren como resueltos.  
5. **Cerrar** los defectos con la evidencia correspondiente.  
6. Informar los defectos cerrados al líder para la elaboración del **informe de defectos**.  

---

## Ejercicio

**Objetivo:**  
Detectar y registrar los defectos presentes en la pantalla de **ingreso de datos del pasajero** en:  
[https://www.blazedemo.com/purchase.php](https://www.blazedemo.com/purchase.php)

**Instrucciones:**  

1. Diseñar un **diagrama de flujo** (círculo de decisión) que represente el proceso de ingreso de datos.  
2. Identificar **todos los caminos posibles** en el flujo.  
3. Crear **un caso de prueba por cada camino**.  
4. Ejecutar los casos de prueba y documentar **cada defecto encontrado** usando la planilla de bugs.  
5. Mantener la **trazabilidad** entre casos de prueba, requisitos y defectos.  

---

[⬅️ Volver al índice del módulo](../modulo3_gestion_defectos.md) | [🏠 Menú principal](../README.md)
