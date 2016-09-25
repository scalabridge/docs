<!-- next_step "arrays" -->

# Loops

Computers are like robots. They are good at doing things over and over and over and over again.

A LOOP is when we ask a program to do something many times.

# loop

If you want something to keep going forever, use a special loop called a `while` loop.

    while (true) {
      println("Hello")
    }

* The `while` statement keeps checking the expression

  * if it's `true` then it loops back
  * if it's `false` then it stops looping and goes on to the rest of the program

To stop it, hold down the CONTROL key and press the C key.

**Note well!** The lines between `{` and `}` are INDENTED. Indentation is very important to you and other humans. It lets our eyes follow the patterns and helps us quickly see what parts of the program go with each other.


# One Infinite Loop

![One Infinite Loop](img/one-infinite-loop.jpg)

*Fun Fact:* The address of Apple HQ is

    1 Infinite Loop
    Cupertino, CA 95014

*Image from the Wikimedia Commons, licensed under the Creative Commons Attribution-Share Alike 3.0 Unported license. Attribution: Joe Ravi*

# LAB: Infinite Hello

Let's change `hello.scala` so that it keeps saying hello over and over again.

    while (true) {
      println("What is your name?")
      val name = readLine()
      println("Hello, " + name + "!")
    }

# LAB: Infinite Food

Write a program called `food.scala` that

1. asks the user for a food -- say, "pizza"
2. prints "Yum, I love pizza!"
3. asks again, and prints again, forever and ever

Remember, CONTROL-C means "Stop everything!!!"


# Who wants to loop forever?

Next, we will change your `food.scala` program so that if the user types "return" -- meaning the string is empty -- then the program exits.

# Exiting a Loop

Our `while` loop assumes that the condition is `true`. This is a keyword that will -- you guessed it -- always be true.
If we want to exit the loop when the input is empty, we'll have to change the condition.

We can use a variable to do this! But first we have to introduce a new concept...

# `val` vs `var`

So far we've been using the keyword `val` to indicate a variable. It's called `val` because
it's short for "value", which means that it can never change.

If you want a variable that can change, you can signal that by using the keyword `var`

**NOTE** The REPL let's you change `val`, try it yourself:

    val x = "foo"
    val x = "bar"

This works just fine! **BUT!** The REPL is a special case, and most of the time you'll be code from source files.
Try putting the below code in a new source file named `test.scala` and running it:

File contents:

    object TestingThis extends App {
      val x = "foo"
      val x = "bar"
      println(x)
    }

Now run:

    scalac test.scala

What happens?

    test.scala:6: error: x is already defined as value x
      val x = "bar"
        ^
    one error found

## Why `val`

When you set something to a value it never changes, this is kind of nice to know! In some ways,
it makes your programs simpler, you know that once you set `val color = "blue"`, color will always be blue!

Being able to change a variable is useful in a handful of situations, loops being one.

## Using `var`

You can initialize a variable in the same way you would for `val`:

    var x = "foo"

To reassign it, leave off the `var` keyword:

    x = "bar"

Now try rewriting `test.scala` with vars so you can change the value of x!

# LAB: Exiting a Loop

Change your `food.scala` program so that if the user types "return" -- meaning the string is empty -- then the program exits.

Hint: Use a `var` to replace the condition in your while loop.

# LAB: Good Food, Bad Food

* Change `food.scala` so that it doesn't love every food.
* If it's a food you like (let's say, pizza), make it print "Yum! I love pizza."
* If it's a food you like (let's say, cabbage), make it print "Yuck! I hate cabbage."

# For loops

Another loop is called `for`, and it's used to loop over a fixed range.

Try this in the REPL:

    for (count <- (1 to 3)) println("Hip! Hip! Hooray!")

Let's unpack this:

* `1 to 3` means that we'll loop over numbers 1, 2, and 3

# Counting in a loop

Remember this poem?

    1 potato
    2 potato
    3 potato
    4
    5 potato
    6 potato
    7 potato
    More

We're going to examine a few different ways to code this.

# `for` with a counter

Try this:

    for (count <- (1 to 4)) {
      println(count.toString + " potato")
    }

`count` means

> "the `count` variable points to the current value of the counter"


# `while` with a counter

    var count = 1
    while(true) {
      println(count.toString + " potato")
      count = count + 1
    }

Whoops! Hit Control-C and join me on the next slide...

# `while` with a counter -- fixed

    var count = 1
    while(count <= 4) do
      println(count.toString + " potato")
      count = count + 1
    end

This is fairly complicated, so let's stop here and make sure to understand everything that's happening in this little program.

# `while` breakdown (pt.1)

    var count = 1

creates a *variable* named `count` and sets its value to `1`.

    while (count <= 4)

starts a loop and immediately compares `count` to `4`.

`1` is less than `4`, so the expression is `true`, so we continue with the loop.

# `while` breakdown (pt.2)

      println(count.toString + " potato")

prints the current value of count (and the word "potato").

      count = count + 1

*increments* the `count` variable... it was `1`, so now it's `2`

That's all - now it goes *back to the `while` line* and checks again

# `while` breakdown (pt.2)

    while (count <= 4)

compares `count` to `4`.

`2` is less than `4`, so the expression is `true`, so we continue with the loop.

Eventually, `count` becomes `5`, and the `while` expression is `false`, and so we stop looping and go on.

# LAB: One Potato

Write a program called `potato.scala` that prints the entire potato poem, accurately.

# Lab: Adder

Write a program named `adder.scala` that keeps a *running total*.

For example:

    scalac adder.scala
    scala ScalaAdder
    1
    Total: 1
    2
    Total: 3
    4
    Total: 7
    -5
    Total: 2


