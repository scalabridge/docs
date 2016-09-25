<!-- next_step "logic" -->

# Input and Output

* Computers have many senses -- keyboard, mouse, network card, digital camera, etc. Collectively, these are called INPUT.

* Computers can also express themselves in many ways -- text, graphics, sound, network, printers, etc. Collectively, these are called OUTPUT.

* Input and Output together are called **I/O**.

# Terminal I/O

* In Scala,
    * `println()` means "print a line to the terminal"
    * `scala.io.StdIn.readLine()` means "read a line from the terminal"

* `readLine` reads all the characters from the keyboard and puts them into a new string, until you press RETURN
* if you don't want to type in `scala.io.StdIn` every time, you can "import" the `readLine` method with:

    import scala.io.StdIn.readLine

# LAB: Hello, friend!

1. Open `hello.scala` in your text editor
2. Change it to contain the following code:

    import scala.io.StdIn.readLine

    object HelloFriend extends App {

      println("What is your name?")
      val name = readLine()
      println("Hello, " + name + "!")

    }

3. Save the file and switch back to the terminal
4. Run the program using the following commands:

    scalac hello.scala
    scala HelloFriend

5. Type in your name and press the RETURN (or ENTER) key

# LAB: Capitalization

* What happens if you type your name in all lowercase?
* Make the program capitalize your name for you even if you forget.

# LAB: Crazy Name

* Now go crazy and make it do all sorts of silly things to your name!

# LAB: Full Name

* Write a program named `name.scala` that asks two things:
  1. Your first name
  2. Your last name
* Then it says hello to the user by her *full name*.
* Run the program by typing:
    scalac name.scala
    scala HelloFriend

# CONGRATULATIONS!

> You just wrote a program!

You are now officially a coder. HIGH FIVE!

# Lab: Name Length

* Change `name.scala` so it also prints the number of characters in the user's name.
* For instance:

        What is your first name?
        Cady
        What is your last name?
        Heron
        Hello, Cady Heron!
        Your name is 9 characters long.

# Advanced Lab: Age

* Ask for your friend's age
* Tell them how old they will be in 10 years
* What happens if they don't enter a number?

