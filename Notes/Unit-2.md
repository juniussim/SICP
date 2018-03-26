# Notes

- If after going through Chapter 1, you yearn for a more layman understanding of what abstraction is, the definitions below would help. 

- In software engineering and computer science, abstraction is a technique for arranging complexity of computer systems. It works by establishing a level of simplicity on which a person interacts with the system, suppressing the more complex details below the current level.

-  Definition from stack:  https://stackoverflow.com/questions/21220155/what-does-abstraction-mean-in-programming

    - Abstracting something means to give names to things, such that the name captures the core of what a function or a whole program does.

    - If i ask you to draw a square, you would know how to do it.

    - A square is an abstraction of "draw four equal lines perpendicular to each other conencted together at a corner".

    - Imagine, everytime i want to have you draw a square, i would have to tell you a detailed steps of drawing four equal lines ... That would be really slow and efficient.

    - Thus, the first benefit of abstraction is that it allows me to get things done way quicker. I can simply say draw a square instead of saying a long list of instructions.

    - The second is that it allows me to be more expressive. We identified special shapes and gave it unique names. We can see the world of geometry in terms of these special shapes and patterns of lines instead of just a bunch of unnamed collection of lines. Our vocabulary increases, and we can also express ourselves in terms of these shapes & patterns rather than just lines. This leads to the third benefit.

    - It allows us to compose larger abstractions from two or more abstractions. We can define a house in terms of a triangle and a square. We can define a village as multiple houses next to each other. We can define a city as multiple villages near one another.

    - Going back to programming, abstractions allow us to write programs that are shorter, easier to write and read. For programs, there is also the added benefit of modularity and reusability.

## Part 2: Building Abstractions with Data

- Recap of Part 1

    - Concentrated on processes and the role of procedures in program design

    - We saw how to use primitive data (numbers) and primitive operations (arithmetic operations) 

    - How to combine procedures to form compound procedures through composition, conditionals, and the use of parameters, and how to abstract procedures by using define

    - Saw that a procedure can be regarded as a pattern for the local evolution of a process. Author phrases this section in a weird way that i still don't quite understand. He explored two key types of processes - namely a recursive and an iterative process (loops).

    - Saw that higher-order procedures enhance the power of our language by enabling us to manipulate, and thereby to reason in terms of, general methods of computation.

    - Much of the essence of programming is captured in the concepts above. 

- What's coming in Part 2

    - Programs are typically designed to model complex phenomena, and more often than not one must construct computational objects that have several parts in order to model real-world phenomena that have several aspects.
    
    - In this part of the book, we will look at more complex data. We will combine data objects to form compound data.

    - Why do we want compound data in a programming language?

        - For the same reasons we want compound procedures:

            - elevate the conceptual level at which we can design our programs

            - increase the modularity of our designs

            - enhance the expressive power of our language (equivalent to elevating the conceptual level)

    - Just as the ability to define procedures enables us to deal with processes at a higher conceptual level than that of the primitive operations of the language, the ability to construct compound data objects enables us to deal with data at a higher conceptual level than that of the primitive data objects of the language

    - Further elaboration will come as i better understand the materials covered in this section

#### Introduction to Data Abstraction

-  Procedure abstraction: separate the way the procedure would be used from the details of how the procedure would be implemented in terms of more primitive procedures.

- Data abstraction: enables us to isolate how a compound data object is used from the details of how it is constructed from more primitive data objects.

- Basic idea of data abstraction:

    - structure the programs, that use compound data objects, so that they operate on 'abstract data'.

    - define a 'concrete' data representation independent of the programs that use the data.

    - the interface between these two parts of our system will be a set of procedures, called *selectors* and *constructors*, that implement the abstract data in terms of concrete representation.

    - To illustrate this technique, we will consider how to design a set of procedures for manipulating rational numbers.

#### Example: Arithmetic Operations for Rational Numbers

- Lets say we want to do arithmetic with rational numbers

    - we want to ble able to add, subtract, multiply and divde rational numbers and test whether two rational numbers are equal.

- Using a useful abstraction technique known as *wishful thinking*

- We start by asumming that we already have a way of:

    - constructing a rational number from a numerator and a denominator.

    - extracting (selecting) its numerator and denominator.

- And that the constructors and selectors are available as procedures:

```clojure
# Constructor

(make-rat <n> <d>) returns the rational number who numerator is the integer <n> and whose denominator is the integer <d>

# Selectors

(numer <x>) returns the numerator of the rational number x

(denom <x>) returns the denominator of the rational number x
```

- Once we have the constructors and selectors for rational numbers, we can express its mathematical rules as procedures.

<p text-align="center">
    <img src="../diagrams/rational-numbers.png"  alt="rational numbers diagram"/>
</p>

- 