<!-- next_step "loops" -->

# Truthiness

Computers have a very strict idea of when things are *true* and *false*.

![Truthiness](img/truthiness.png)

(Unlike Stephen Colbert...)

# True or False?

Try the following in the Scala REPL:

* `1 < 2`
* `2 + 2 < 4`
* `2 + 2 <= 4`
* `"apple".isEmpty`
* `"".isEmpty`

# Conditions

The magic word `if` is called a CONDITIONAL.

    if (age < 18) {
      println("Sorry, adults only.")
    }

# if... then... else...

The magic word `else` allows BRANCHING.

    if (age >= 18) {
      println("allowed")
    } else {
      println("denied")
    }

Like a fork in the road, the program chooses one path or the other.

# 2 + 2 = 4

Sadly, this expression:

    2 + 2 = 4
    
causes an error with a really weird message. You need to do

    2 + 2 == 4

instead. Why?

# The Tragedy of the Equal Sign

* a single equal sign means ASSIGNMENT
  * `val name = "Alice"` -- "assign the variable 'name' to the value 'Alice'"
* two equal signs means COMPARISON
  * `name == "Alice"` -- "does the variable 'name' contain the string 'Alice'?"

> This is confusing, and you should feel confused.

# LAB: Good Friend, Bad Friend

* Your `hello.scala` program should currently look something like this:

        println("What is your name?")
        val name = readLine()
        println("Hello, " + name + "!")

* Now change `hello.scala` so that it doesn't always say hello!
  * If the user's name is "Darth" then say "Go away!"

# Conjunction Junction

* You can make more complicated logical expressions using operators like:
  * `X && Y` means "are both X and Y true?" (`&&` pronounced 'and')
  * `X || Y` means "is either X or Y (or both) true?" (`||` pronounced 'or')
  * `!X` means "is X false?" (think about it) (`!` pronounced 'not')

* For example:

        if (age > 5 && age <= 18) {
          println("You're probably in school!")
        else
          println("You're not in school!")
        end

# LAB: Enemies List

* Change `hello.scala` so that it says "Go away!" if the user's name is any one of a number of evil names
* For instance, Voldemort, Satan, Lex Luthor...


