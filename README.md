# Sistema de Gestión de Biblioteca - OOP en C#

## Introducción
Desde la editorial Puñetas, dedicada a temas legales, nos han pedido un sistema de gestión de la biblioteca para manejar sus libros en el lenguaje de C#. Para realizar este ejercicio deberemos aplicar la OOP (programación orientada a objetos) a medida que vamos realizandolo.

## Requisitos
- Sube el código para todas las instrucciones a tu repositorio.
- Aplica la OOP.

## Instrucciones
### Iteración 1: Crear Libros
Creamos una clase `Book` con tres propiedades: `Title` (título del libro), `Author` (autor del libro) y `Year` (año de publicación). Implementamos un constructor que inicializa todas las propiedades.

### Iteración 2: Funcionalidades Adicionales
Añadimos la función `IsOlderThan(int year)` que compara el año de publicación del libro con un año dado, y la función `UpdateYear(int newYear)` que actualiza el año de publicación del libro.

### Iteración 3: Categorización de Libros
Creamos un enum `Genre` con algunas categorías de libros y añadimos una propiedad opcional `Genre` de tipo `Genre` a la clase `Book`. Introducimos una nueva propiedad `IsBestseller` en la clase `Book`.

### Iteración 4: Información Detallada del Libro
Implementamos la función `BookInfo` que devuelve una cadena de texto con información detallada sobre el libro, incluyendo título, autor, año de publicación y género del libro.

### Iteración 5: Asignación de Géneros
Asignamos géneros a algunos de los libros creados y utilizamos la función `BookInfo` para imprimir la información detallada de cada libro.

### Iteración 6 : Bestsellers
Modificamos la función `BookInfo` para que también indique si el libro es un bestseller.

### Iteración 7: Ampliación de la Clase EBook
En esta iteración, ampliamos la clase `EBook` para incluir funcionalidades específicas de los libros electrónicos, como la capacidad de descargar y leer el libro.

### Iteración 8: Implementación de la Interfaz IPrintable
En esta iteración, implementamos la interfaz `IPrintable` en la clase `Book` para proporcionar una forma estándar de imprimir información sobre el libro. También creamos otras clases, como `Magazine`, `Newspaper`, etc., que implementan esta interfaz y proporcionan su propia implementación del método `PrintInfo`.
