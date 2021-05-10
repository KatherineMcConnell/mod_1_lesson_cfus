# Variables, Arguments, and Return Values

## Check for Understanding

#### What is a method? An argument? A return value?

  *  Method - a set of instruction. Built in or class methods allow us reuse code and manipulate it. There are query and command methods.
  Query fetches information and command changes or gives
  a behavior to the class.

  * Arguments - are the specific input to a method or instance inside parenthesis () to use or manipulate it.
    An argument "passes" specific data

  * Parameters - are generic placeholders input to a method or instance inside parenthesis () to use or manipulate it.

  * Default Arguments??

  * Return Value - is the output of a method. Every method has exactly one return value.
  A return value is not the same as printing. They are either defined explicitly using the "return" keyword or  is the last line of code run.

  * Variables - Keywords which we pick and we create to hold or point to return values that we want to maintain and re-use.

#### What keywords do we use to create methods?

  * The "class" keyword before the class name tells ruby to
    make a class called....

  * The "def" keyword before a method tells ruby to define  a new method called...

  * The "end" keyword closes the method. At the very end of your methods you also have to close your class.

  * Variable are keyword we use to hold onto return value that we want to perhaps reuse. Variables are also assigned to objects.

#### How does Ruby know what to return from a method?

  * Ruby reads top to bottom. The last line of a method, before the closing "end" unless it is specifically told to "return" at a specific line. Then it stops reading at that line and returns the result of that line.

#### How do you call one method from within another method?

  * You can call one method within another as long as they
    are in the same class. You can call any method in the
    class above or below and ruby will find it.
    ie: "Hello".size. Size is a method that can be used inside a method because it is a built-in method in

  * You can also
    call methods from the attr_reader & accessor initialized
    attribute methods.

  * You can also call methods from other
    classes given a placeholder representing an argument
    in that separate class with the method called not on
    the separate class but on the placeholder name.

#### Why do we use methods?

  * We use methods to reuse code. Methods are called on objects aka instances of classes.

  * Methods can be passed arguments to manipulate instantiated attributes of a class.

  * Built in methods are organized by data type ie string, integer, etc.

#### What is abstraction?

  * Abstraction (noun) is simply put pulling out functionality &  hiding complexity.

  * Abstracting (verb)
