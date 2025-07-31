# Laboratorio adicional 4 - Resuelto

## Solución del ejercicio 1 👤

### Personas menores a 18 y mayores a 65

TÉCNICA DE PARTICIÓN EQUIVALENCIA Y ANÁLISIS DE VALOR LÍMITE (por ser un campo numérico).
X = Edad

**Técnica de partición:**

| Partición   | Rango/Valor    | Resultado |
| ----------- | -------------- | --------- |
| X ≤ 18      | Rango válido   | ✔️        |
| X ≥ 65      | Rango válido   | ✔️        |
| 18 < X < 65 | Rango inválido | ❌        |
| CP1: X = 15 | Menor a 18     | Positivo  |
| CP2: X = 70 | Mayor a 65     | Positivo  |
| CP3: X = 40 | Entre 18 y 65  | Negativo  |

**Técnica de valores límites:**

| Caso | Valor               | Resultado |
| ---- | ------------------- | --------- |
| CP4  | X = 18              | Positivo  |
| CP5  | X = 65              | Positivo  |
| CP6  | X = 19              | Negativo  |
| CP7  | X = 64              | Negativo  |
| CP9  | X = alfabético      | Negativo  |
| CP10 | X = caracteres esp. | Negativo  |
| CP11 | X = nulo            | Negativo  |

---

### Pago con impuestos según días de retraso (10% hasta 15 días, 15% hasta 30 días, 25% hasta 60 días)

X = días
Técnica de partición:

| Rango       | Resultado                                                   |
| ----------- | ----------------------------------------------------------- |
| X ≤ 15      | Rango válido (10%)                                          |
| 16 ≤ X ≤ 30 | Rango válido (15%)                                          |
| 31 ≤ X ≤ 60 | Rango válido (25%)                                          |
| X > 60      | No sabemos que pasa pero hay que consultar con el funcional |
| X ≤ 0       | No sabemos que pasa pero hay que consultar con el funcional |
| CP1: X = 4  | Rango válido                                                |
| CP2: X = 20 | Rango válido                                                |
| CP3: X = 49 | Rango válido                                                |
| CP4: X = 0  | No sabemos que pasa pero hay que consultar con el funcional |
| CP5: X = 61 | No sabemos que pasa pero hay que consultar con el funcional |

**Supuestos:**

- El número de días de retraso se autocalcula luego de ingresar el número de documento del cliente.
- Si el cliente tiene saldo a favor, el número de días de retraso será negativo.

**Fuera de alcance:**

- No clientes o personas no registradas.

**Técnica de valores límites:**

| Caso | Valor | Resultado     |
| ---- | ----- | ------------- |
| CP6  | X:15  | ÉXITO - 10%   |
| CP7  | X:16  | ÉXITO - 15%   |
| CP8  | X:30  | ÉXITO - 15%   |
| CP9  | X:60  | ÉXITO - 25%   |
| CP10 | X:31  | ÉXITO - 15%   |
| CP11 | X:61  | No lo sabemos |
| CP12 | X:0   | No lo sabemos |

**Código de provincias**
TÉCNICA DE PARTICIÓN DE EQUIVALENCIA Y ANÁLISIS DE VALOR LÍMITE

CP1: X = 0
CP2: X = 1
CP3: X = 15
CP4: X = 24
CP5: X = 25

**Supuesto:**

- El código de provincia es un campo numérico que solo admite dos dígitos (no admite caracteres especiales ni letras). Los valores válidos son del 1 al 24.

**Acceso por Login y Password (usuario y clave)**
Tabla de decisiones:

|         | CP1 | CP2 | CP3 | CP4 |
| ------- | --- | --- | --- | --- |
| USUARIO | T   | F   | T   | F   |
| CLAVE   | T   | T   | F   | F   |

---

## Solución del ejercicio 2

**_Proceso de compra de una cartera:_**

- El usuario ingresa a la página con su usuario y contraseña, selecciona el producto que quiere comprar, coloca la cantidad y procede a darle al botón comprar, donde ingresa los datos del envío y métodos de pago.

**_Técnicas de caja negra aplicadas_**

- **Métodos de pago:** TRANSICIÓN DE ESTADO
- **Cantidad de unidades que desea comprar:** PARTICIÓN DE EQUIVALENCIAS Y ANÁLISIS DE VALOR LÍMITE
- **Compra - general:** CASO DE USO
- **Login (usuario y contraseña):** TABLA DE DECISIÓN
- **Información de valida código postal (Argentina):** PARTICIÓN DE EQUIVALENCIAS Y ANÁLISIS DE VALOR LÍMITE

---

[⬅️ Volver al índice del módulo](../modulo1_principios_fundamentos.md) | [🏠 Menú principal](../README.md)
