# Desafío — Resolución

## Ejercicio 1

**Casos de prueba principales:**

- **CP1 (Positivo):** Ingresar valores válidos  
  - Área: alfabética  
  - Sección: numérica  
  - Línea: alfabética  
  - Producto: alfabético  
  - Descripción: alfabética

- **CP2 (Negativo):** Ingresar valores inválidos  
  - Área: numérica  
  - Sección: alfabética  
  - Línea: numérica  
  - Producto: numérico  
  - Descripción: numérica

- **CP3 (Negativo):** Probar combinaciones inválidas, incluyendo campos nulos y símbolos especiales.

---

## Ejercicio 2

**Casos de prueba principales:**

- **CP1 (Positivo):** Ingresar CUIL válido y contraseña válida → acceso exitoso.
- **CP2 (Negativo):** Ingresar CUIL inválido → mensaje de login inválido.
- **CP3 (Negativo):** Ingresar CUIL válido y contraseña inválida → mensaje de contraseña incorrecta.
- **CP4 (Positivo):** Probar otras opciones válidas dentro del sistema.

---

## Ejercicio 3

**Casos de prueba principales:**

- **CP1 (Positivo):**  
  - Producto existente  
  - Cantidad numérica válida (según stock disponible)  
  - Precio unitario numérico con 2 decimales  
  - Validar que el precio total sea cantidad × precio unitario

- **CP2 (Positivo):** Seguir probando combinaciones con valores límite según especificaciones.

- **Casos negativos:**  
  - Partición de equivalencia con valores fuera de rango o formatos incorrectos.

---

Puedes revisar la solución completa en el siguiente archivo:  
[laboratorios/desafio.pdf](laboratorios/desafio.pdf)

---

[⬅️ Volver al índice del módulo](../modulo2_Casos%20de%20prueba.md) | [🏠 Menú principal](../README.md)
