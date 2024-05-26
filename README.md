# OOP Basics en CSharp: Sistema de Gestión de Biblioteca

## Introducción
En este ejercicio, crearemos un sistema de gestión de biblioteca para manejar libros. Definiremos una clase `Book` para describir las propiedades de los libros, como el título, el autor y el año de publicación. También incluiremos funcionalidades para actualizar los detalles de un libro, comparar libros y mostrar información sobre cada libro.

## Requisitos
- Sube el código para todas las instrucciones a tu repositorio.

## Instrucciones

### Iteración 1: Crear Libros
1. Crea una clase `Book` con tres propiedades: `Title` (título del libro), `Author` (autor del libro) y `Year` (año de publicación).
2. Implementa un constructor que inicialice todas las propiedades. Por defecto, establece el año de publicación en 2000.
3. Crea al menos tres objetos de la clase `Book` con diferentes libros. Al inicializarlos, asegúrate de usar valores predeterminados y también especificar el año manualmente en al menos uno de los objetos.

### Iteración 2: Funcionalidades Adicionales
1. Crea una función `IsOlderThan(int year)` que compare el año de publicación del libro con un año dado. Debe devolver `true` si el libro es más antiguo que el año dado, y `false` en caso contrario.
2. Implementa una función `UpdateYear(int newYear)` que actualice el año de publicación del libro.
3. Realiza comparaciones de años de publicación entre los libros creados y llama a la función `UpdateYear` varias veces para ver cómo cambian los libros.

### Iteración 3: Categorización de Libros
1. Crea un enum `Genre` con algunas categorías de libros, como `Fiction` (ficción), `NonFiction` (no ficción), `Science` (ciencia), `Fantasy` (fantasía), etc.
2. Agrega una propiedad opcional `Genre` de tipo `Genre` a la clase `Book`.
3. Introduce una nueva propiedad `IsBestseller` en la clase `Book`. Esta propiedad será `true` si el libro es un bestseller, y `false` en caso contrario.

### Iteración 4: Información Detallada del Libro
1. Implementa una función `BookInfo` que devuelva una cadena de texto con información detallada sobre el libro.
2. La cadena debe incluir el título, el autor, el año de publicación y el género del libro. Si el género no está definido, debe indicar que es desconocido.

### Iteración 5: Asignación de Géneros
1. Asigna géneros a algunos de los libros creados.
2. Utiliza la función `BookInfo` para imprimir la información detallada de cada libro.

### Iteración 6 (Bonus): Bestsellers
1. Modifica la función `BookInfo` para que también indique si el libro es un bestseller.
2. La cadena devuelta debe tener dos partes: una sobre el estado de bestseller del libro y otra sobre su género.
