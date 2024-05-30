# Sistema de Gestión de Biblioteca - OOP en C#

## Introducción
Desde la editorial Puñetas, dedicada a temas legales, nos han pedido un sistema de gestión de la biblioteca para manejar sus libros en el lenguaje de C#. Para realizar este ejercicio deberemos aplicar la OOP (programación orientada a objetos) a medida que vamos realizandolo.

## Requisitos
- Sube el código para todas las instrucciones a tu repositorio.
- Aplica la OOP.

## Instrucciones

### Prepara el proyecto
Abre un terminal desde la carpeta raíz del proyecto:
1. Añade un fichero gitignore con el comando:
   ```bash
   dotnet new gitignore
   ```
2. Crea la solución con el comando:
   ```bash
   dotnet new sln -n PunyetasBooks
   ```
3. A continuación crea un proyecto dentro de la misma carpeta:
   ```bash
   dotnet new console -n PunyetasBooks
   ```
4. Añade el proyecto a la solución con el comando:
   ```bash
   dotnet sln add ./PunyetasBooks/PunyetasBooks.csproj
   ```

### Iteración 1: Crear la clase Book
1. Crea un nuevo fichero dentro de la carpeta del proyecto `./PunyetasBooks` con el nombre `Book.cs`.
2. Dentro del fichero `Book.cs`, sigue los siguientes pasos:
   1. Crea un `namespace` `PunyetasBooks`
   2. Crea una clase `Book`
   3. Añade tres propiedades:
        - `Title` (título del libro),
        - `Author` (autor del libro) y
        - `Year` (año de publicación).
   4. Implementa un constructor que inicialice todas las propiedades.

Para crear la clase puedes seguir la [documentación oficial](https://learn.microsoft.com/en-us/dotnet/csharp/fundamentals/tutorials/classes)

### Iteración 2: Añadir funcionalidades Adicionales a Book

1. Añade el método `IsOlderThan(int year)`
   - Debe comparar el año de publicación del libro con un año dado y devuelva true si el año de publicación es anterior al año pasado por parámetro.
2. Añade el método `updateYear(int newYear)`
   - Este método no devuelve nada y debe actualizar el año de publicación del libro.

### Iteración 3: Añadir generos literarios (Book Genres en inglés) para categorizar los libros
1. Añade un enum `Genre` a la clase `Book` con algunos géneros de libros (Fiction, NonFiction, Biography), puedes ampliar la lista con los que consideres.
2. Añade una propiedad opcional `Genre` de tipo `Genre` a la clase `Book`.
3. Introduce una nueva propiedad `IsBestseller` de tipo bool a la clase `Book`.

### Iteración 4: Información Detallada del Libro
1. Añade el método `getBookInfo`:
   - Debe retornar una cadena de texto con la información detallada sobre el libro: título, autor, año de publicación y género del libro.

### Iteración 5: Crea el programa
Modifica el fichero `Program.cs` con las siguientes funcionalidades:
1. Añade 3 libros que tú elijas
2. Modifica cada uno de los libros asignándole el género apropiado
3. Utiliza el método `BookInfo()` de cada libro para devolver la información detallada de cada libro.
4. Corre el proyecto para comprobar que funciona correctamente. (_tip: busca el comando necesario para correr el proyecto ;)_)

### Iteración 6 : Bestsellers
Modifica el método `BookInfo` para que también indique si el libro es un bestseller.

### Iteración 7: Crea la clase EBook
1. Crea un nuevo fichero en el proyecto con el nombre de `EBook.cs`.
2. Dentro del fichero añade la clase `EBook`. Esta clase debe extender las funcionalidades `Book` con algunos métodos espécificos de los libros electrónicos:
   - Crea el método `downloadEbook()`:
     Debe retornar un string: "El libro <BOOK TITLE> ha sido descargado con éxito"
   - Crea una propiedad `pageNumber` de tipo numérico:
   - Crea el método `readEBook()`
     Este método debe aumentar el número de página cada vez que sea invocado y devolver el string: "Has leído la página <pageNumber> "

### Iteración 8: Implementación de la Interfaz IPrintable

En esta iteración, implementamos la interfaz `IPrintable`
- Crea un fichero `IPrintable.cs` con el método `printInfo()`.
- Implementa el interfaz `IPrintable` en la clase `Book` para proporcionar una forma estándar de imprimir información sobre el libro.
- Crea las clases: `Magazine` y `Newspaper` que extiendan de `Book` e implementen el método `PrintInfo`. Elige tú la salida que quieras del método.


