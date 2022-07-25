# SOLID y Clean Code

La deuda técnica es la falta de calidad en el código y que lleva a incrementar los costos económicos.

- Tiempo de mantenimiento
- Tiempo de refactorizar código
- Tiempo de comprender código
- Tiempo adicional en la transferencia del código

### Esquema de la deuda técnica

- Imprudente: No hay tiempo, solo copia y pega.
- Inadvertida: ¿Qué son los patrones de diseño?
- Prudente: Tenemos qué entregar rápido, ya refactorizaremos. Ahora sabemos cómo lo deberíamos haber hecho.

Puede ser normal e inevitable.
Debemos ser consientes y pagar la deuda.

_Refactorización: Entendible y tolerante a cambios. Pruebas automáticas._

Alguien termina pagando la deuda.
"Código limpio es aquel que se ha escrito con la intención de que otra persona (o tú mismo en el futuro) lo entienda.

## Nombres proununciables y expresivos.

Ausencia de información técnica en los nombres.

- ❌ interface UserInterface
- ✅ interface User

No exagerar o ser redundante en los nombres.

Nombres según el tipo de dato.

- ✅ _fruits_ Si se trata de un array de valores.
- ✅✅ _fruitNames_

Booleans: Evitar las negaciones en el nombre.

- ✅ open: isOpen
- ✅ active: isActive
- ✅ fruit: hasFruit
- ✅ noValues: hasValues

Numbers

- ✅ fruits: maxFruits, minFruits, totalFruits.
- ✅ cars: totalOfCars

Funciones: Deben representar acciones.
El verbo que representa la acción, seguida del sustantivo.

- Create user if not exists: createUser
- Update user if not empty: updateUser

Leer y comprender facilmente.
Usar el sentido semántico.

Classes

- El nombre es lo más importante de la clase.
- Formado por un sustantivo o frases de sustantivo.
- No demasiado genéricos.
- UpperCamelCase
- ¿Qué hace exactamente la clase?
- ¿Cómo exactamente esta clase realiza cierta tarea?
- ¡Hay algo especifico sobre su ubicación?

````
## Proyecto de práctica

Este es un proyecto de Vanilla TypeScript en Vite, para trabajar los ejercicios del curso de Principios SOLID y Clean Code.}

### Despliega el proyecto

Clonar o descargar el proyecto.

Instalar dependencias.

```
yarn install
ó
npm install
```

Ejecutar el proyecto.

```
yarn dev
ó
npm run dev
```
````
