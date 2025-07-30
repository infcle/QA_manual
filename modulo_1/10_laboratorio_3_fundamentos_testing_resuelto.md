# Laboratorio 4: Fundamentos del Testing - Resuelto

## Solución del Ejercicio 1

### 1. El Testing muestra la presencia de fallas

El testing puede mostrar la presencia de fallas, pero no su ausencia. Nuestro trabajo es identificar fallas. Si un tester no detecta fallas, puede significar que:

- El desarrollo es perfecto (lo cual es poco probable).
- No está realizando las pruebas suficientes o correctas.

**Ejemplo:** Si se está revisando el botón de arrepentimiento de MercadoLibre y el tester evalúa la creación de usuario o el login, es probable que no encuentre fallas porque no está probando lo que se modificó. Si no detecta fallas, las encontrará el usuario.

---

### 2. La exhaustividad no es posible

No se puede probar todo. Siempre se debe priorizar lo más importante y trabajar con muestras representativas.

**Ejemplo:** Nos piden que en un ticket de compra figure un renglón con el porcentaje del IVA. No se puede controlar cada ticket, por lo que se selecciona una muestra para evaluar.

---

### 3. Detección temprana de fallas

Mientras más temprano se detecten las fallas, mejor. Detectarlas en etapas iniciales reduce el re-trabajo y los costos asociados.

**Ejemplo:** Si una falla se encuentra mientras se revisa el requerimiento, el re-trabajo es mucho menor que si se detecta días antes de la entrega al usuario.

---

### 4. Agrupamiento de defectos

Cuando se detecta una falla en una funcionalidad, es probable que existan más fallas relacionadas. Es importante seguir probando esa funcionalidad para reportarlas todas.

**Ejemplo:** En un formulario con veinte campos, si uno no valida correctamente, es probable que otros también tengan problemas. No basta con reportar un solo error.

---

### 5. Paradoja del pesticida

Las pruebas deben actualizarse para seguir siendo efectivas. Reutilizar pruebas es una buena práctica, pero deben adaptarse a los cambios en el sistema.

**Ejemplo:** Si se realizaron pruebas hace tres meses y el cliente solicita un cambio, el tester debe considerar las actualizaciones necesarias para que las pruebas sigan siendo relevantes.

---

### 6. Las pruebas dependen del contexto

El enfoque de las pruebas varía según el contexto, como el navegador, el sistema operativo o la metodología utilizada.

**Ejemplo:** Un juego puede funcionar perfectamente en Android, pero no ejecutarse en iOS.

---

### 7. La ausencia de fallas es una falacia

No se puede garantizar que un sistema esté 100% libre de fallas. Las pruebas se enfocan en lo más importante dentro del tiempo disponible.

**Ejemplo:** La exhaustividad es imposible, por lo que las fallas menores pueden corregirse con el tiempo y mediante actualizaciones.

---

## Solución personal del laboratorio

Puedes consultar el enunciado original aquí:  
[📄 Descargar laboratorio_3.pdf](../material/laboratorio_3.pdf)

---

[⬅️ Volver al índice del módulo](../modulo1_principios_fundamentos.md) | [🏠 Menú principal](../README.md)
