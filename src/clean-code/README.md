# Clean Code

## Nombres proununciables y expresivos.

Ausencia de información técnica en los nombres.

- ❌ interface UserInterface
- ✅ interface User

No exagerar o ser redundante en los nombres.

Nombres según el tipo de dato.

- ✅ _fruits_ Si se trata de un array de valores.
- ✅✅ _fruitNames_

### Booleans

Evitar las negaciones en el nombre.

- ✅ open: isOpen
- ✅ active: isActive
- ✅ fruit: hasFruit
- ✅ noValues: hasValues

### Numbers

- ✅ fruits: maxFruits, minFruits, totalFruits.
- ✅ cars: totalOfCars

### Funciones

Deben representar acciones.
El verbo que representa la acción, seguida del sustantivo.

- Create user if not exists: createUser
- Update user if not empty: updateUser

Leer y comprender facilmente.
Usar el sentido semántico.

### Classes

- El nombre es lo más importante de la clase.
- Formado por un sustantivo o frases de sustantivo.
- No demasiado genéricos.
- UpperCamelCase
- ¿Qué hace exactamente la clase?
- ¿Cómo exactamente esta clase realiza cierta tarea?
- ¡Hay algo especifico sobre su ubicación?

### Funciones, argumentos y parámetros

Sentido entre nombre y contenido.

Parámetros: Cuando definimos la función.
Argumentos: Cuando usamos / invocamos a la función.

- Las funciones deben hacer solo una tarea.
- La simplicidad es fundamental.
- Funciones de tamaño reducido.
- Funciones de una sola línea sin causar complejidad.
- Menos de 20 líneas en funciones. Opcional.
- Evitar el uso del "else".
- Priorizar uso de la condicional ternaria.

## Principio DRY

_Si quieres ser un programador productivo, esfuerzate en escribir código legible. - Robert C. Martin._

**Don't Repeat Yourself**

- Evitar duplicidad de código.
- Simplifica las pruebas.
- Ayuda a centralizar los procesos.
- Código autoexplicativo.

## Estructura recomendada de una clase.

Comenzar con lista de propiedades.

1. Estáticas
2. Públicas
3. Privadas
4. Métodos
   1. Constructores estáticos / Método estático
   2. Constructor
   3. Métodos estáticos
   4. Métodos privados
   5. Resto de métodos ordenados por importancia
   6. Getters y Setters al final

## Comentarios en el código

- Cuando usamos código de terceros, librerias, api, etc. Comentamos el porqué de su uso.
- Explicar < Auto explicativo
- No comentes el código mal escrito, reescribe el código.

## Uniformidad en el proyecto

- Problemas similares, soluciones similares.
- Formas de nombrar funciones, archis, carpetas, etc.
- Misma estructura de archivos.
- Indentación.

## Acronimo STUPID

**Code Smells**: Algo no anda bien.

- Singleton: Patrón singleton: Contras del contacto global.
- Tight Coupling: Alto acoplamiento.
- Unestability: Código sin unit tests.
- Premature optimization: Optimizaciones prematuras.
- Indescriptive naming: Nombres poco descriptivos.
- Duplication: Duplicidad de código, no usar DRY.
- Bajo acoplamiento y alta cohesión.

_Queremos diseñar componentes que sean auto contenidos, auto suficientes e independientes. Con un objetivo y un propósito bien definido - The pragmatic Programer._

- La cohesión se refiere a lo que la clase, o módulo, puede hacer.
- La baja cohesión significaría que la clase realiza gran cantidad / variedad de acciones. Sin enfoque.
- Alta cohesión: La clase está enfocada en solo métodos relacionados con la intención de la clase.

### Acoplamiento

Se refiere a cuán relacionadas o dependientes son dos clases o módulos entre si.

- Bajo acomplamiento: Cambiar algo en una clase, no debería afectar otras.
- Alto acoplamiento: Dificultaría los cambios y el mantenimiento.

### Optimizaciones prematuras

No debemos anticiparnos a los requisitos y desarrollar abstracciones innecesarias que puedan añadir complejidad accidental.

**Solución minima indispensable**

### Nombres poco descriptivos

- Ser muy especifico o demasiado genérico.
- Cuántos WTF por mínuto? xD

### Duplicidad de código

- Real: Código identico con la misma función.
- Accidental: Código similar con funciones distintas. Trabajar con parámetros y optimización.

## Code Smells

- Inflación: Métodos grandes o sub métodos pequeños. Clases largas a clases pequeñas más enfocadas.
- Obsesión Primitiva: Resolver problemas solo con datos primitivos.
- Lista larga de parámetros: Más de 3 o 4 parámetros en un método. Transformar en sub métodos y/o objetos.

### Acopladores

- Feature Envy: Una clase usa más la información de otras clases que las propias. Mantener las cosas relacionadas juntas.
- Intimidad inapropiada: Clases que usan demsaiado un método en particulas. Separar el método.
- Cadenas de mensajes: Demasiadas llamadas de un lado a otro. Reducir cantidad de dependencias.
- Middle Man: Evitar clases que solo delegan de una clase a otra. Evitar pasos innecesarios.
