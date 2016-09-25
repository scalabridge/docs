<!-- next_step "hashes" -->

# args

There's a magic list named `args`.

It contains the *command line arguments* to the program.

If the user types:

    scala hello.scala Alice Bob

then args contains:

    List("Alice", "Bob")

# Command-Line Hello

Change `hello.scala` to contain:

    println("Hello, " + args(0))

and run it a few times, e.g.

    scala hello.scala Alice

try running it without providing an argument:

    scala hello.scala

oh no!

    java.lang.ArrayIndexOutOfBoundsException: 0

# LAB: Safe Hello

Change `hello.scala` so it won't throw an exception if there isn't any input.

# LAB: Hello, Everyone!

Change `hello.scala` to say hello to *every one* of its command line arguments.

For instance:

    scala hello.scala Alice Bob Charlie
    Hello, Alice!
    Hello, Bob!
    Hello, Charlie!

# LAB: Add

Write a program named `add.scala` that adds all of its command line arguments together.

e.g.

    scala add.scala 1 2 3
    6

Do you remember how to convert a string to an integer?



