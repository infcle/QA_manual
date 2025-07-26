# Desafío - Resuelto

Ejemplo de resolución del desafío:

## Escenario: Registro de usuario

### Caso de Prueba 1

- **ID:** CP-01
- **Descripción:** Verificar registro exitoso con datos válidos
- **Precondición:** Usuario no registrado
- **Pasos:**
  1. Ingresar datos válidos en el formulario
  2. Hacer clic en 'Registrar'
- **Resultado esperado:** Mensaje de éxito y usuario creado

### Caso de Prueba 2

- **ID:** CP-02
- **Descripción:** Validar error al registrar con email existente
- **Precondición:** Email ya registrado
- **Pasos:**
  1. Ingresar email ya registrado
  2. Completar el resto de los datos
  3. Hacer clic en 'Registrar'
- **Resultado esperado:** Mensaje de error indicando email duplicado
