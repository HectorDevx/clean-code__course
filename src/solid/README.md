# Principios SOLID

Nos indican cómo organizar nuestras funciones y estructuras de datos en componentes y cómo dichos componentes deben estar interconectados. Son principios no reglas.

## Principio de responsabilidad única

Tener una única responsabilidad !== Hacer una única cosa.

### Detectar incumplimiento del Single Responsability Principle

- Nombres de clases o módulos demasiado genéricos.
- Cambios en el código suelen afectar la clase o módulo.
- La clase involucra multiples capas.
- Número elevado de importaciones.
- Cantidad elevada de métodos públicos.
- Excesivo número de líneas de código.

## Principio abierto cerrado

Depende mucho del contexto. Abiertas para la extensión, cerradas para la modificación.
Fácil de adaptarse a los cambios sin tener que modificar los métodos desde su raíz.

### Detectar incumplimiento del Principio abierto cerrado

- Cambios afectan a la clase o módulo.
- Cuando una clase o módulo afecta muchas capas.

## Principio de sustitución de Liskov

_"Siendo U un subtipo de T, cualquier instancia de T debería poder ser sustituida por cualquier instancia de U sin alterar las propiedades del sistema"_

## Principio de segregación de interfaz

_"Los clientes no deberían estar obligados a depender de interfaces que no utilicen."_

### Detectar incumplimiento del Principio de segregación de interfaz

- Si las interfaces que diseñamos nos obligan a violar los principio de responsabilidad única y sustitución de Liskov.

## Principio de inversión de dependencias

- Los módulos de alto nivel no deben depender de módulos de bajo nivel.
- Ambos deberían depender de abstracciones.
- Las abstracciones no deberían depender de detalles.
- Los detalles deberían depender de las abstracciones.

**Arquitectura Hexagonal**
Nos referimos a clases abstractas o interfaces.

- +Aumentar la tolerancia al cambio.
- -Inyección de dependencias.
  Controlar funcionalidades desde un lugar / archivo en concreto.
