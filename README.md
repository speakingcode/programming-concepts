Programming Concepts
====================
## Concepts and Topics for New and Experienced Programmers to Learn, Practice, and Master.
## Copyright @speakingcode (http://speakingcode.com)
## Creative-Commons Attribution-ShareAlike 4.0 International License (CC BY-SA 4.0)

## Intro
This book is intended to introduce various concepts, practices, tools and philosophies in order to provide a more guided path for seriously exploring the art of programming and the ways of coding. It is not intended to provide mastery of each of the topics, but rather to explain them just enough to allow the reader to guide his or her self with direction and confidence through the crowded landscape of computing. Instead of being a tutorial for a specific set of technologies, it is a detailed outline of many of the kinds of weapons available in the programmer's arsenal, sprinkled with tidbits of experience, wisdom and hisorical context where appropriate.

Although largely conceptual and agnostic from any particular language, platform, or software package, some concrete examples may be used to reinforce concepts or emphasize practical constraints. It is not intended to teach any specific language or tool, but examples may be biased in favor of preferred implements.

## What Is Programming

## Basic Programming

There are many applications of programming and various languages emphasize different paradigms, styles, and approaches that make use of different techniques and concepts to best suit their purposes. Regardless, several basic programming concepts are nearly universal to most languages used in modern practice. Although exact syntax and behavior will vary, many languages treat them conceptually quite similarly.

### Variables

Similar to variables in mathematics, variables in programming are symbolic names used to reference pieces of data that may change or vary. In computing terms, variables are references that point to specific segments of memory. In practical terms, variables are names we give to pieces of data and use to recall and act on that data later on. 

Perhaps more important than variables themselves are the data they point to. Variables can reference simple values like numbers or strings of text, as well as more complex structures like collections and abstract objects that have properties and actions. The data that variables point to has a _type_ which determines the possible value(s) the data can hold and what operations can be done with it (and also tells the computer how to store it and manage it in memory). Different languages have different _type systems_ that deal with types differently.

#### Primitive Types

Primitive types, or basic types, are the most basic kinds of values we can work with in programs; they are usually provided by the language itself ('built in') and are the basic building blocks that more complex types of data are composed from. The available primitive types vary from language to language.

Although different language compilers and interpreters represent primitive types (and more generally, any type) of data 'behind the scenes' differently from one another, some common representations (particularly from the C family of languages) are described below. It is not important to memorize such low-level details, but it is important to appreciate the practical limitations inherent to them.

##### Integer

Integers are numbers with no fractional/decimal component which can be positive or negative. Integers typically support numerical operations like addition, subtraction, multiplication, and integer division (where the remainder is disregarded), as well as conversion to other numerical types.

Some languages, like C and Java, have a variety of integer types, such as `int`, `short`, and `long`, the difference being the amount of space the data takes up in memory and the range of possible values. Larger types like `long` take up more memory (and require more work for the CPU to read and operate on), but have a much larger range of possible values, where smaller types use less memory but have a smaller range of values.

##### Decimal/Float

Decimals/Floats are numbers with fractional/decimal components which can be positive or negative. Their representation is more complex than integers, similar to scientific notation. 'Float' indicates that the position of the decimal point is not fixed; the number of decimal digits varies. Because of how floats are stored in memory, some calculations may yield a loss of precision, producing small 'rounding errors'.

Similarly to integer types, many langauges have multiple decimal types, such as `float` and `double`, again with varying sizes of memory allocation and range of values/precision.

##### Char

Some languages have a char type, which, in contrast to numerical types, represents a single character of text. A char may be a letter, a numerical character, punctuation, a space, or even special characters like newline or tab characters. Char representation in memory and the possible values varies depending on platform specifics and encoding (UTF-8, UTF-16, ASCII etc.) Common operations for chars include changing from lowercase to uppercase (and vice-versa), and comparing by lexigraphical order, which is used often for searching through and sorting text.

##### String

Strings are collections of letters, symbols, spaces, numbers etc. joined together and treated as a unit of text. Common operatons for strings include concatenation (joining two or more strings together), finding substrings, removing substrings, inserting substrings, breaking strings down into substrings, getting the length of a string, comparing them, and so on. String values are typically denoted with quotation marks: `"this is a string"`.

Languages that have a _char_ type usually treat strings as collections of chars, but languages such as Ruby only have strings (a string of length 1 is effectively a char).

##### Boolean

Booleans are true/false values: they can be either `true` or `false`, and nothing else. They are useful for logical conditions, flags/indicators, and "on-off" switches. The result of most comparison operations is a boolean value (`8 < 16`  => true, `name == "John Doe"`  => false, `x <= y`, etc.) Some languages treat other, non-boolean types as _truthy_ or _falsey_, where the value may be treated as true or false, but conventions vary. In C, boolean values are simply `ints`, where 0 is false and all other values are true. In JavaScript, `null`, `undefined`, `NaN` (Not-a-Number, the result of invalid numerical operations such as division by 0), `""` (empty strings), `false`, and `0` are all falsey, but any object, array, non-empty string, non-zero number, and `true` are truthy. In Ruby, only `nil` (Ruby's version of null) and `false` evaluate to false while any other value of any type is true.

##### null, nil, undefined
In most languages, variables can exist that don't actually have or point to a value yet; variable _declaration_ and variable _assignment_ are treated as separate operations. Under the hood, decalring a variable tells the computer to reserve a space of memory for the variable, and assignment actually puts a value there. Most languages use a special value called `null` as the "default" non-existent value. The concept of null takes different forms, such as `nil` in Ruby. Some languages also use a similar but distinct value if the code references a variable that hasn't even been declared, such as `undefined` in JavaScript. These special values are useful for programmers in many cases.

#### Collections

##### Array/List
##### Dictionary/hash/associative array
  
#### Loops
##### While
##### For

#### Execution Flow
##### if, else, else if
##### switch/case

#### Functions
##### Defining functions
##### calling functions
##### return values
##### parameters
###### pass-by-value
###### pass-by-reference

  event-driven programming
    asynchronous operations
    callbacks


Object Oriented Programming
  classes/objects
  member variables/fields
  methods
  message passing/method calls
  interfaces
  inheritence
  polymorphism
  encapsulation
  cohesion
  coupling

  OOP design principles
    KISS
    DRY
    SOLID
      single repsonsibility principle
      open/closed principle
      liskov substitution principle
      interface segregation principle
      dependency inversion principle
    GRASP
    packaging/namespacing
    abstraction/refactoring
    design patterns
      singleton
      factory
      command
      decorator
      iterator
      memento
      dependency injection
      observer/publish-subscribe
      ...


Data Structures & Algorithms
  ADTs
  arrays
  circular arrays
  linked-lists
  doubly-linked lists
  hashes/maps
  stacks
  queues
  trees
  binary trees
  balanced trees
  r/b-trees
  heaps
  tries
  
  run-time complexity
    asymptotic bounds/big oh
    operation costs (insert, remove, append, find)
  
  sorting
    insertion sort
    bubble sort
    merge sort
    quick sort
    heap sort
    bucket sort
  
  searching
    binary search
  
  recursion
  dynamic programming

Databases
  relational
    tables
    primary keys
    foreign keys
    data integrity
    cascade operations
    views
    normalization

    SQL
      insert
      update
      select
      delete
      joins

    PostgreSQL
    MySql

  non-relational/no-sql
    key-value stores
      redis, etc.
    document databases
      mongodb, etc.
  
Web/Enterprise
  HTTP
    GET
    POST
    PUT
    DELETE
  REST
  JSON
  XML
  SOAP (ew?)

Programming in Practice

  general
    interpreters/repl shells
    compilers
    
  reuse
    libraries/modules/packages
foss
    
  architecture/platform
    frameworks
    SDKs

  version control
   svn, cvs, 
mercurial
    git
      commit
      stash
      branch
      merge
      fork
      ...

  debuggers
    break points
    step through/into
    inspection
    ...

  grep/regex/pattern matching

## C
defacto low level merits of creators, capabilities of the language, nature of the computing scene, chance

Unix/Linux
