# Principios SOLID 📚

SOLID es un acrónimo que representa cinco principios de diseño orientados a objetos que, cuando se combinan, hacen que el software sea más comprensible, flexible y mantenible.

Claro, exploremos los principios SOLID en detalle:

### 1. Single Responsibility Principle (SRP)
- **Detalles**: Cada clase en un programa debe tener una sola responsabilidad. Evita que una clase maneje múltiples funcionalidades.
- **Implementación**: Descomponer clases grandes en clases más pequeñas, cada una enfocada en una funcionalidad específica.
- **Ejemplo**: En lugar de tener una clase `Empleado` que gestione tanto los detalles personales como los informes de desempeño, se tendría una clase para manejar los detalles personales y otra para los informes.

### 2. Open-Closed Principle (OCP)
- **Detalles**: Las entidades de software deben ser abiertas para extensión, pero cerradas para modificación. Esto significa que deberías poder agregar nuevas funcionalidades sin cambiar el código existente.
- **Implementación**: Uso de interfaces y clases abstractas para permitir que los comportamientos se extiendan sin modificar la clase existente.
- **Ejemplo**: Si tienes una clase de filtro de productos, en lugar de modificarla cada vez para agregar un nuevo criterio, podrías crear nuevos filtros que implementen una interfaz de filtro común.

### 3. Liskov Substitution Principle (LSP)
- **Detalles**: Las clases derivadas deben ser sustituibles por sus clases base, lo que significa que los objetos de una clase derivada deben comportarse de la misma manera que los de la clase base, sin alterar el funcionamiento del programa.
- **Implementación**: Asegurarse de que las subclases no sobreescriban comportamientos esperados de la clase base.
- **Ejemplo**: Si tienes una clase `Pájaro` con un método `volar()`, una subclase como `Pingüino` (que no puede volar) no debería invalidar este comportamiento.

### 4. Interface Segregation Principle (ISP)
- **Detalles**: Los clientes no deben ser forzados a depender de interfaces que no utilizan. Esto previene que las interfaces tengan métodos que no se aplican a todas sus clases implementadoras.
- **Implementación**: Crear interfaces específicas y más pequeñas que sean implementadas por clases, en lugar de una sola interfaz grande.
- **Ejemplo**: En lugar de una interfaz grande `Trabajador` con métodos como `trabajar()` y `comer()`, se pueden tener interfaces separadas para distintas responsabilidades.

### 5. Dependency Inversion Principle (DIP)
- **Detalles**: Los módulos de alto nivel no deben depender de los de bajo nivel; ambos deben depender de abstracciones. Además, las abstracciones no deben depender de detalles; los detalles deben depender de las abstracciones.
- **Implementación**: Utilizar inyección de dependencias para invertir el control, permitiendo que las dependencias de alto nivel especifiquen sus dependencias de bajo nivel a través de abstracciones.
- **Ejemplo**: Un objeto `ReportGenerator` (alto nivel) no debería depender directamente de una clase `DataAccess` (bajo nivel), sino de una interfaz `IDataAccess`.

---

## Referencias 🌐🔗

- [FreeCodeCamp - The SOLID Principles of Object-Oriented Programming Explained in Plain](https://www.freecodecamp.org/news/solid-principles-explained-in-plain-english/)
- [DigitalOcean - SOLID: The First 5 Principles of Object Oriented Design](https://www.digitalocean.com/community/tutorials/solid-principles-of-object-oriented-design)
- [GeeksforGeeks - SOLID Principle in Programming: Understand With Real Life Examples](https://www.geeksforgeeks.org/solid-principle-in-programming-understand-with-real-life-examples/)
- [Baeldung - A Solid Guide to SOLID Principles](https://www.baeldung.com/solid-principles)

NOTA: Se han creado algunos ejemplos de cada principio SOLID con diferentes lenguajes de programación en el siguiente [repositorio](https://github.com/AngelGerardoMolinaValdez/roadmap-software_architecture.git)

---

### [Responde el cuestionario 📝](../../../cuestionario/02-principios_de_disenio/principios_basicos/SOLID.md)

### [Volver al temario 🏡](../../../readme.md)
