Programming Concepts
====================
## Concepts and Topics for New and Experienced Programmers to Learn and Master.
## Copyright @speakingcode (http://speakingcode.com)
## Creative-Commons Attribution-ShareAlike 4.0 International License (CC BY-SA 4.0)

## Intro
This guide is intended to introduce many programming concepts, practices and tools and philosophies of programming technique, approach, and style in order to provide a clear, holistic path for deeply exploring the art of programming. It is not intended to provide mastery of each of the subjects, but rather to explain them just enough to allow the reader to guide his or her self with direction and confidence through the myriad sources of information available elsewhere. Think of this document as a detailed outline of many of the weapons available in the programmer's arsenal, sprinkled with tidbits of experience, wisdom and hisorical context where appropriate.

Although I aim to keep the document largely conceptual and agnostic from any particular language, platform, or software package, some concrete examples may be used to reinforce concepts or emphasize practical constraints. It is not my intent to teach any specific language or tool, but there is no guarantee that I will not be biased in favor of my own preferred implements.


## Basic Programming

There are many applications of programming and various paradigms, styles, and languages that make use of different techniques and concepts to best suit their purposes, but several basic programming concepts are universal to many or nearly all languages used in modern practice. Although the exact syntax and behavior will vary, many common programming languages treat them conceptually quite similarly.

### Variables

Similar to variables in mathematics, variables in programming are symbolic names used to reference pieces of data. In computing terms, this means variables are symbols that refer or point to segments of memory. In practice this means they are names we give to pieces of data and use to recall and act on that data later on. Variables have values, which can change, i.e. vary.

More important than variables themselves are the data they point to. Variables can reference simple values like numbers or strings of text, as well as more complex structures like collections and objects with properties and actions. Variables have _type_ which indicates the kind of data they point to. Different languages have different _type systems_ and handle variable types differently, but generally type impacts what kind of information the data can hold and what _operations_ can be done on it. 

#### Primitive Types

Primitive types are the most basic kinds of values we can handle distinctly in programs; they are provided by the language itself and are the basic building blocks that more complex types of data are made from. Which primitive types exist varies from language to language, and some languages like Ruby don't even truly have distinct primitive types (everything is an object in Ruby), but conceptually they are widely present in most languages.

Although different language compilers and interpreters represent primitive types (and more generally, any type) of data differently from one another, some common representations (particularly from the C family of languages) are described below. It is not important to memorize such low-level details, but it is important to appreciate the practical limitations inherent to them. 

##### Integer

Integers are numbers with no fractional/decimal component which can be positive or negative. In many languages integers are stored in memory as 4-byte values, or 32 bits, giving them a range from 0 to (2^32) - 1 (unsigned) or -(2^31) to (2^31) - 1 (signed). Integers typically support numerical operations like addition, subtraction, multiplication, and integer division (where the remainder is disregarded), as well as conversion to other numerical types.  

##### Decimal/Float

Decimals/Floats are numbers with fractional/decimal components which can be positive or negative. They are often represented as 4-byte values, or 32 bits, but the representation is more complex than integers, similar to scientific notation. 'Float' refers to the fact that the position of the decimal can 'float'; the number of decimal digits varies. Because of how floats are stored, sometimes precision can be lost producing small 'roudning errors' in some calculatons. 

##### Char

Some languages have a char type, which, in contrast to numerical types, represents a single character of text. A char may be a letter, a numerical character, punctuation, a space, or even special characters like newline or tab characters. Char representation in memory varies depending on platform specifics and encoding (UTF-8, UTF-16, ASCII etc.), but they are still ultimately numbers stored as bytes, meaning the CPU operates on them like numbers. Common operations for chars include changing from lowercase to uppercase and vice-versa and comparing (used for sorting text).

##### String

Strings are collections of chars (letters, symbols, spaces, etc.) joined together and treated as text. Common operatons for strings include concatenation (joining two or more strings together), finding substrings, removing substrings, inserting substrings, getting their length, breaking down into substrings, and so on. Strng values are typically enclosed in quotation marks: `"this is a string"`

##### Boolean

Booleans are true/false values: they can be either `true` or `false`, and nothing else. They are useful for logical conditions, "on-off" switches, etc. Whenever two values are compared (equals, less-than, greater-than, etc.) the result of the comparison is a boolean value. Some languages treat other, non-boolean types as _truthy_ or _falsey_, but conventions vary. In C, boolean values are simply ints, where 0 is false and all other values are true. In JavaScript, `null`, `undefined`, `NaN` (the result of invalid numerical operations such as division by 0), `""` (empty strings), `false`, and `0` are all falsey, but any object, array, non-empty string, non-zero number, and `true` are truthy. In Ruby, only `nil` (Ruby's version of null) and `false` are false, any other value of any type is true.

##### null, nil, undefined

In most languages, variable _declaration_ and variable _assignment_ are two separate operations, meaning it is possible to have variables that exist but don't actually point to a value. Generally, `null` is the "default" non-existent value. It is sometimes called `nil`, such as in Ruby. Some languages go a bit further and have a distinct value used when a program references a variable that hasn't even been declared, such as `undefined` in JavaScript. These special values are useful for programmers. 

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
