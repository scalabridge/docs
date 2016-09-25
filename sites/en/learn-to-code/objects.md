<!-- next_step "strings" -->

# Objects

An OBJECT is a location in computer memory where you can store DATA (aka VALUES).

There are many kinds of objects, including String, Int, Double, List, Map... 

(The different kinds of objects are called CLASSES or TYPES. Some day soon you will create your own classes but for now, we will use the built-in ones.)

# Int

An `Int` is short for "Integer" which is a whole number.

    10
    -12
    540698

# Double

A `Double` is a way to express numbers with decimals.

    3.0
    -1.23
    4.89034851

Try typing the above numbers into the REPL to see what result type comes back!
    
    scala> 3
    res0: Int = 3

    scala> -1.23
    res1: Double = -1.23

# Strings

A STRING is an object that's a collection of characters, like a word or a sentence.

    "apple"
    "banana"
    "Cherry Pie"

# Lists

A List is an ordered collection of things, with the caveat that the things all must be the same type of thing.

    List(1, 2, 3, 4)
    List("foo", "bar", "baz")

# Types

In Scala, objects can have types. These types are very specific, which is why there's a difference between
`Int` and `Double`. When you type something into the REPL, you see its type come back with the result.

# Methods

Methods allow you to perform actions on the objects.

    "apple".toUpperCase

The `toUpperCase` method turns `"apple"` into `"APPLE"`.

The type of the object determines which methods you can perform, try:

    4.toUpperCase

# Return Values

Every time a method is executed, it returns a response.

You can think of it as the answer to a question. 

    2 + 2          # Question: What is 2 + 2?
    res0: Int = 4  # Answer: 4

    "apple".toUpperCase  
    # Q: What is the uppercase of the string "apple"?
    
    res1: String = APPLE
    # A: the string "APPLE"

