<!-- next_step "argv" -->

# Lists

* An LIST is a CONTAINER
  * an object that contains other objects
* It's a list of objects

# What makes an list a list

* You can put any objects inside it, as long as they're the same type!
* In any order
* They stay in order
* Duplicates are fine

Lists are super useful for storing data! You'll see these everywhere.

# Creating an list

    List("apple", "banana", "cherry")

# List Indexes

* Every slot in the list has a serial number
* You can retrieve any item in an list by its INDEX
* An index is a number from 0 to infinity
  * actually to the size of the list

# List Indexes Exercise

Try this in the Scala REPL:

    val fruits = List("apple", "banana", "cherry")
    fruits(1)

Did you get the result you expected?

Why or why not?

# Start At Zero

When counting, 

humans start at one, 

but **computers start at zero**.

So the first item in an list is number zero, not number one.

# The End

Try this:

    fruits(99)

Uh oh! 

    java.lang.IndexOutOfBoundsException: 99

What happened? The computer tried to locate the index, but there was nothing there, so it
threw an exception. Because of this, we always try to write our programs in a way so that
we only access an element if we know it's there.

# List Methods

    fruits.last
    fruits.first
    fruits.reverse

# Turning an list into a string

    fruits.mkString
    fruits.mkString(",")
    fruits.mkString(" and ")

Note that `toString` doesn't work the way you might expect on lists:

    println(fruits.toString)

# Looping through an list

    fruits.map { fruit =>
      println(fruit)
    }

* `map` is like `while` or `for` for lists
* `fruits.map` means "for each item inside this list, let's do something"
* `fruit =>` means "put the current item into a variable named `fruit`"
* `println(fruit)` means "print out the value of this variable"
* and that's the end of the loop! :-)

# Lab: reverse fruit

Given this list:

    val fruits = List("apple", "banana", "cherry")

write a program that prints:

    yrrehc
    ananab
    elppa

# Setting items in an list

// TODO - see Dagny's comment: https://github.com/scalabridge/curriculum/issues/28

You can't! Lists are immutable!

# Checking an list

The `contains` method checks if an object is inside an list or not.

    fruits.contains("apple")
    res0: Boolean = true
    
    fruits.contains("pizza")
    res5: Boolean = false

# LAB: enemies list refactoring

I'd like you to **refactor** your old `hello.scala` program to use the `contains` method to check if someone is your enemy.

# TODO: more list labs


