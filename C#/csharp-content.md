# C# Learning Roadmap

## 🧱 Week 1 - C# Basics

### Language Fundamentals
- [ ] What is .NET and CLR (very high level)
- [ ] Installing SDK + using dotnet CLI
- [ ] Project structure
- [ ] Program.cs
- [ ] Main() entry point
- [ ] Build vs Run

### Syntax Core
- [ ] Variables and data types
  - int, double, float, decimal, bool, string, char
- [ ] Type inference with `var`
- [ ] Constants with `const`
- [ ] Operators
  - Math, comparison, logical

### Control Flow
- [ ] if / else
- [ ] switch
- [ ] for / while / do-while
- [ ] foreach
- [ ] break / continue

### Methods
- [ ] Method declaration
- [ ] Parameters and return types
- [ ] Optional parameters
- [ ] Method overloading
- [ ] ref, out, in parameters

### Basic Types Deep Cut
- [ ] Value types vs Reference types
- [ ] struct vs class
- [ ] string immutability

### Arrays & Collections Intro
- [ ] Arrays
- [ ] List\<T>
- [ ] Dictionary<TKey, TValue>

### Console Stuff
- [ ] Console.ReadLine()
- [ ] Console.WriteLine()
- [ ] Parsing input
  - int.Parse
  - TryParse

## 🧱 Week 1–2 - Intermediate C#

### OOP in C#
- [ ] Classes and objects
- [ ] Fields vs properties
- [ ] Constructors
- [ ] Access modifiers
  - public, private, protected, internal
- [ ] Encapsulation
- [ ] Inheritance
- [ ] Polymorphism
- [ ] virtual / override
- [ ] Abstract classes
- [ ] Interfaces

### Properties
- [ ] Auto properties
- [ ] Getters/setters
- [ ] Backing fields

### Static World
- [ ] static classes
- [ ] static methods
- [ ] static constructors

### Namespaces
- [ ] Creating and organizing them
- [ ] using directives

### Exception Handling
- [ ] try / catch / finally
- [ ] Custom exceptions
- [ ] When to throw

### Generics
- [ ] List\<T>
- [ ] Generic methods
- [ ] Generic classes
- [ ] Constraints
  - where T : class, etc

### Collections Proper
- [ ] List
- [ ] Dictionary
- [ ] HashSet
- [ ] Queue
- [ ] Stack
- [ ] IEnumerable

### LINQ
- [ ] Where
- [ ] Select
- [ ] OrderBy
- [ ] First / FirstOrDefault
- [ ] Any / All
- [ ] GroupBy
- [ ] Projection

### Delegates & Events
- [ ] delegate basics
- [ ] Func / Action
- [ ] Events pattern

### Lambda Expressions
- [ ] (x) => x * 2

### Nullable Types
- [ ] int?
- [ ] null checks
- [ ] null-coalescing operator `??`
- [ ] null conditional `?.`

### Enums

### File I/O
- [ ] Reading/writing text files
- [ ] JSON serialize/deserialize
  - System.Text.Json

## 🧠 Week 3 - Advanced C#

### Async Programming
- [ ] async / await
- [ ] Task
- [ ] Task\<T>
- [ ] ConfigureAwait (basic awareness)
- [ ] Why blocking is bad

### Dependency Injection
- [ ] Constructor injection
- [ ] Interfaces for services
- [ ] Loose coupling

### SOLID Principles
- [ ] Single Responsibility
- [ ] Open Closed
- [ ] Liskov Substitution
- [ ] Interface Segregation
- [ ] Dependency Inversion

### Advanced OOP Topics
- [ ] Records
- [ ] Immutability patterns
- [ ] Composition over inheritance
- [ ] Extension Methods
- [ ] Attributes
- [ ] Reflection (basic idea)
- [ ] IDisposable + using statement

### Unit Testing Basics
- [ ] xUnit or NUnit
- [ ] Arrange Act Assert
- [ ] Mocking basics (Moq)

## 🗃 Week 3 - Repository Pattern + IMDb Console App

### Repository Pattern Concepts
- [ ] What is a repository
- [ ] Why abstraction over data access
- [ ] Interface + implementation split
- [ ] CRUD operations
- [ ] Generic repository (optional)

### Example Mental Model
```c#
interface IMovieRepository {
    void Add(Movie movie);
    Movie GetById(int id);
    IEnumerable<Movie> GetAll();
    void Update(Movie movie);
    void Delete(int id);
}

Implementation MovieRepository : IMovieRepository
```

### Layered Architecture
- [ ] Models / Entities
- [ ] Repositories
- [ ] Services
- [ ] UI (Console layer)

### Dependency Injection Wiring
- [ ] Inject repository into service
- [ ] Inject service into program

### IMDb Console App Features
- [ ] Add movie
- [ ] List movies
- [ ] Search movie
- [ ] Update movie
- [ ] Delete movie
- [ ] Save/load from file or JSON

### Bonus Points
- [ ] LINQ queries for search
- [ ] Async file operations
- [ ] Validation layer
- [ ] Unit tests for repository

## ⚡ Fast Learning Order (Compressed Mode)

1. C# syntax + control flow
2. Classes + OOP
3. Collections + LINQ
4. Interfaces + DI
5. async/await
6. Repository pattern
7. Build console CRUD app
8. Add file persistence
9. Add tests