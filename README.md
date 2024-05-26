# OOP Basics in CSharp: Library Management System

## Introduction
In this exercise, we will create a library management system to handle books in a library. We will define a `Book` class to describe the properties of books. We will also include functionalities to update book details, compare books, and display information about each book.

After completing this lab, you will be able to:
- Create a class with properties, defined with and without default values, as well as optional properties.
- Create a constructor with some of its input parameters having a default value.
- Instantiate objects of a class using different constructors.
- Pass values from one object to a function of another.
- Use enums for categorization.

## Requirements
- Upload the code for all of the following prompts to your repository.

## Submission
Upon completion, run the following commands:
```
git add .
git commit -m "done"
git push origin main
```

## Starter code
No initial code provided.

## Iterations

### Iteration 1
1. Create a class `Book` with three properties: `Title` (string), `Author` (string), and `Year` (int).
2. Create a constructor for all of the properties. Set the `Year` input parameter within the constructor to have a default value of 2000.
3. Create a few of your own books as objects of the `Book` class (minimum 3). When initializing them, at least one of the objects should use the default `Year` value and at least one should have its `Year` defined manually within the constructor.

### Iteration 2
1. Create a function `IsOlderThan(int year)` that takes an input parameter and compares it to the `Year` property. It returns a `bool` value as a result of the comparison if the `Year` property is less than the input parameter.
2. Create a function `UpdateYear(int newYear)` that updates the `Year` property.
3. Compare the `Year` of any of your created `Book` objects at least 2 times and print the results.

### Iteration 3
1. Create a new enum `Genre` and give it a few possible values (like `Fiction`, `NonFiction`, `Science`, `Fantasy`).
2. Create an optional property `Genre` of type `Genre` in the `Book` class.
3. Create a new class property `IsBestseller` that is a `bool` and has a default value `false`.

### Iteration 4
1. Create a function `BookInfo` that returns a `string`.
2. Depending on the value of the property `Genre`, return the string stating the genre of the book. If the property `Genre` is `null`, return a string stating that the genre is unknown.

### Iteration 5
1. Assign genres to some of your books.
2. Use the `BookInfo` function to print the information of each book.

### Iteration 6 (Bonus)
1. Within the `BookInfo` function, if the property `IsBestseller` is `true`, add a message to your return string saying that the book is a bestseller. The previous genre check logic should still happen regardless of this new logic, so the return string should now have two parts - one regarding their bestseller status and the other regarding the genre.

For example, a possible return string would be: `"This book is a bestseller. Genre: Fiction."`
