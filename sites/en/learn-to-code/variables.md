<!-- next_step "the_command_line" -->

# Variables

A VARIABLE is a NAME for an object. You give an object a name using the ASSIGNMENT operator (it looks like an equal sign).

    val color = "blue"
    val fruit = "berry"

The `val` keyword is necessary to give the object a name.

Anywhere you can use an object, you can use a variable instead.

    color + fruit
    fruit.toUpperCase

# The Warehouse Metaphor

![Warehouse from Raiders of the Lost Ark](img/warehouse.jpg)

Think of memory as a giant warehouse.

# The Warehouse Metaphor Explained

If memory is a giant warehouse...

...and *objects* are **boxes** in that warehouse

...then a *value* is the **contents** of a box

...and a *variable* is a **label** you stick on the outside of the box

# Variables are documentation

Which is clearer, this:

    60 * 60 * 24

or this:

    val secondsPerMinute = 60
    val minutesPerHour = 60
    val hoursPerDay = 24
    val secondsPerDay = secondsPerMinute * minutesPerHour * hoursPerDay

?

# Lab: Play In The REPL

Let's spend a few minutes just playing around in the REPL. Some things to try:

* write a poem
* YELL THE POEM
* calculate 2 + 2 and more complicated things
* assign your best friend to a variable
* reverse your best friend's name
* get a new best friend and reverse her too

# The Pointer Metaphor

    val snack = "Apple"

![snack-apple](img/snack-apple.svg)

Think of a variable as **pointing** to an object.

# Many pointers can point to the same thing

    val fruit = "Apple"
    val snack = fruit

![snack-fruit](img/snack-fruit.svg)

After this both `snack` and `fruit`...

  * are *pointing* to the same *object*
  * have the same *value*

# Return values are new

Most methods will return a *new* value

    val fruit = "banana"
    val snack = fruit.toUpperCase

![fruit-banana-snack-banana](img/fruit-banana-snack-banana.svg)

`"banana"` and `"BANANA"` are two *different objects* in memory

