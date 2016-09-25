<!-- next_step "variables" -->

# Numbers

There are a lot of types that represent Numbers, we'll focus on `Int` and `Double`

The following operations work on numbers:

  * + -- addition
  * - -- subtraction
  * * -- multiplication
  * / -- division
  * % -- modulus

# LAB: Playing With Numbers

Answer the following questions using the Scala REPL:

* How many seconds are in an hour?
* How many minutes are in a week?
* How many seconds old are you?
* How many years old is someone who is 1 billion seconds old?

# Order of operations

Q: What is 1 plus 2 times 3?

# Order of operations

Q: What is 1 plus 2 times 3?

A: *It depends!*

  * `(1 + 2) * 3` is 9
  * `1 + (2 * 3)` is 7

# Parentheses Are Free

When in doubt, use parentheses!

# Strings vs. Numbers

Hmmm....

    1 + 2
    "1" + "2"
    "1 + 2"

# Strings plus Numbers

Hmmm again...

    "1" + 2

Huh?!

    res0: String = 12

It can't be both an `Int` and a `String`, so Scala converts the `Int` to a `String` in order to combine them.

You can do this too!

# Type Conversion

There are methods to convert `Int` to `String` and back:

    14.toString
    "14".toInt
    "23.4".toDouble
    "this isn't a number!!".toInt

Try these in the Scala REPL!

# Advanced Number Theory (optional)
# Arithmetic

Try this in the REPL:

    1 + 2
    3 - 4
    5 * 6
    7 / 8

Whoa! What just happened?

# Integer Arithmetic

7 and 8 are *Integers*

so the result is an Integer

7/8 is somewhere between 0 and 1

but there is no integer between 0 and 1

so the computer has to *round down* to 0

# Floating Point Arithmetic

    7.0/8.0

7.0 and 8.0 are *Doubles*

so the result is a `Double`

and `0.875` can fit in a `Double`

# Okay, that's enough math!

