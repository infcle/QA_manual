# 📌 Atributos de un Caso de Prueba

## Contenido

- [Atributos de un caso de prueba](#-atributos-de-un-caso-de-prueba)
- [Planilla de casos de prueba](#️-planilla-de-casos-de-prueba)
- [Planilla de pasos de casos de prueba](#️-planilla-de-casos-de-prueba)
- [Ejercicios de registración](#-ejercicios-de-registración)

---

## ✅ Atributos de un Caso de Prueba

Un caso de prueba debe contener una serie de atributos clave para garantizar una correcta ejecución, seguimiento y análisis de los resultados.

- **ID**: Identificador único del caso.
- **Descripción**: Título breve que indique qué se va a probar.
- **Datos**: Información necesaria para ejecutar el caso.
- **Precondiciones**: Condiciones que deben cumplirse antes de ejecutar el caso.
- **Prioridad / Severidad**: Nivel de importancia del caso.
- **Tipo de caso**: Positivo (camino feliz) o negativo (alternativo, excepción).
- **Resultado esperado**: Descripción de lo que debería ocurrir si todo funciona correctamente.
- **Resultado obtenido**: Resultado real observado tras la ejecución.
- **Postcondiciones**: Estado o condiciones del sistema después de la ejecución.
- **Pasos a ejecutar**: Detalle de acciones secuenciales a seguir.

### 🧾 Ejemplo de atributos de un caso de prueba

- **ID**: 3D-P-CP-001  
- **Descripción**: Comprar 2 entradas para función 3D, viernes 22:00 hs., pago con tarjeta de crédito.  
- **Precondiciones**: Tarjeta de crédito habilitada y con fondos suficientes.  
- **Prioridad / Severidad**: Alta (47% de las compras se hacen con tarjeta de crédito).  
- **Tipo de caso**: Positivo  
- **Resultado esperado**: Emisión de tickets (impresora o PDF).  
- **Resultado obtenido**: Emisión de tickets (impresora o PDF).  
- **Postcondiciones**: Entradas vendidas y facturadas.  
- **Pasos a ejecutar**: Descritos en el documento de pasos (Step by Step).

---

## 🗂️ Planilla de Casos de Prueba

### 📋 Plantilla 1: Caso General

| Atributo              | Descripción |
|------------------------|-------------|
| **ID del CU**          | Identificador mnemotécnico del Caso de Uso |
| **ID del CP**          | Identificador mnemotécnico del Caso de Prueba |
| **Título del CP**      | Breve descripción del caso |
| **Ciclo**              | Ciclo de ejecución de pruebas |
| **Tipo**               | Positivo (camino feliz), Negativo (alternativo, excepción) |
| **Prioridad**          | Nivel de importancia (Alta, Media, Baja) |
| **Severidad**          | Nivel de criticidad (Negocio, Funcional, Formal) |
| **Status**             | Estado del caso (Aprobado, Fallido, En proceso, Anulado, Suspendido) |
| **Precondiciones**     | Condiciones necesarias antes de ejecutar |
| **Postcondiciones**    | Estado del sistema después de ejecutar |
| **Datos generales**    | Datos requeridos para realizar el caso |
| **Resultado esperado** | Resultado que se espera con los datos y ambiente configurados |
| **Resultado obtenido** | Resultado real tras la ejecución |
| **Ambiente de test**   | Entorno donde se ejecuta (servidores, red, infraestructura) |
| **Versión de SW**      | Versión del producto o sistema bajo prueba |
| **Responsable del CP** | Persona encargada del diseño y/o ejecución |
| **Fecha y Hora**       | Momento en que se diseñó y/o ejecutó el caso |

---

### 📋 Plantilla 2: Detalle de Pasos

| Atributo                 | Descripción |
|--------------------------|-------------|
| **ID del CP**            | Identificador mnemotécnico del Caso de Prueba |
| **Número de paso**       | Numeración secuencial del paso |
| **Descripción del paso** | Instrucción clara, concreta y precisa |
| **Precondiciones**       | Condiciones requeridas antes del paso |
| **Datos**                | Valores específicos necesarios para el paso |
| **Resultado esperado**   | Resultado que se debería obtener en ese paso |
| **Resultado obtenido**   | Resultado real obtenido tras la ejecución |
| **Status**               | Estado del paso (Aprobado, Fallido) |
| **Evidencia**            | Captura de pantalla, archivo o cualquier elemento que pruebe la ejecución |

---

## 🧪 Ejercicios de Registración

A continuación se presentan casos de prueba que simulan distintos escenarios del proceso de **registración de usuarios** en una aplicación web. Estos ejercicios permiten evaluar tanto caminos exitosos como fallos comunes en validaciones.

---

### ✅ CP01 - Registración exitosa con datos válidos

- **ID del CP**: REG-CP-001  
- **Título**: Registración con datos válidos  
- **Ciclo**: Prueba funcional básica  
- **Tipo**: Positivo  
- **Prioridad**: Alta  
- **Severidad**: Negocio  
- **Status**: Aprobado  
- **Precondiciones**: Usuario no registrado previamente  
- **Datos generales**:
  - Nombre: Juan Pérez  
  - Email: <juan.perez@example.com>
  - Contraseña: Segura123  
  - Confirmación de contraseña: Segura123  
- **Resultado esperado**: El sistema muestra mensaje de éxito y redirige al login  
- **Resultado obtenido**: El sistema registra correctamente al usuario y redirige  
- **Ambiente de test**: WebApp - Chrome / Firefox / Localhost  
- **Versión de SW**: v1.0.0  
- **Responsable del CP**: QA Elmer  
- **Fecha y Hora**: 2025-08-04 15:00  

---

### ❌ CP02 - Fallo por contraseña débil

- **ID del CP**: REG-CP-002  
- **Título**: Registración con contraseña débil  
- **Tipo**: Negativo  
- **Prioridad**: Media  
- **Severidad**: Funcional  
- **Precondiciones**: Usuario no registrado  
- **Datos generales**:
  - Nombre: Ana Gómez
  - Email: <ana.gomez@example.com>
  - Contraseña: 1234  
  - Confirmación de contraseña: 1234  
- **Resultado esperado**: Mensaje de error: "La contraseña es demasiado débil"  
- **Resultado obtenido**: Mensaje mostrado correctamente  
- **Status**: Aprobado  
- **Ambiente de test**: WebApp - Firefox  
- **Versión de SW**: v1.0.0  
- **Responsable del CP**: QA Elmer  
- **Fecha y Hora**: 2025-08-04 15:10  

---

### ⚠️ CP03 - Fallo por email duplicado

- **ID del CP**: REG-CP-003  
- **Título**: Registración con email ya existente  
- **Tipo**: Negativo  
- **Prioridad**: Alta  
- **Severidad**: Negocio  
- **Precondiciones**: El email ya está registrado  
- **Datos generales**:
  - Email: <juan.perez@example.com>
  - Contraseña: NuevaClave2025  
  - Confirmación: NuevaClave2025  
- **Resultado esperado**: Mensaje: "El email ya se encuentra registrado"  
- **Resultado obtenido**: Mensaje mostrado correctamente  
- **Status**: Aprobado  
- **Ambiente de test**: WebApp - Chrome  
- **Versión de SW**: v1.0.0  
- **Responsable del CP**: QA Elmer  
- **Fecha y Hora**: 2025-08-04 15:20  

---

### 🧪 CP04 - Fallo por campos vacíos

- **ID del CP**: REG-CP-004  
- **Título**: Intento de registración sin completar campos obligatorios  
- **Tipo**: Negativo  
- **Prioridad**: Alta  
- **Severidad**: Formal  
- **Precondiciones**: Página de registro accesible  
- **Datos generales**:  
  - Nombre: [vacío]  
  - Email: [vacío]  
  - Contraseña: [vacío]  
- **Resultado esperado**: Mensajes de validación en los campos vacíos  
- **Resultado obtenido**: Validaciones mostradas correctamente  
- **Status**: Aprobado  
- **Ambiente de test**: WebApp - Chrome  
- **Versión de SW**: v1.0.0  
- **Responsable del CP**: QA Elmer  
- **Fecha y Hora**: 2025-08-04 15:30  

---

[⬅️ Volver al índice del módulo](../modulo2_Casos%20de%20prueba.md) | [🏠 Menú principal](../README.md)
