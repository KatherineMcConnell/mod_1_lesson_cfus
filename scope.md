# Scope

## Check for Understanding

#### In Class Notes With Ian:

 * Ruby reads top to bottom. It's either 'learning' code (ie, definition of a class/method/variable) or it's 'executing' code(ie runner file)

 * Variables
  * can only be accessed within our current scope, or deeper
  * eg, a variable defined in  a method can be used anywhere in that method, but not outside the method
  * eg, a variable defined inside a block can be used in that block, but not outside of the block(exceptions unless we return it, or pass in as a parameter)

  * Methods
    * Ruby can call methods that it has already 'learned'
    * methods cannot share variables, but we could pass them as parameters/return values exception instance variables.

  * Classes
    * usually one class in a file by itself with no 'executable' code
    * instance variables can be declared anywhere in our class definition
    * instance variables are available to any method in our class
    * if you try to use an instance variable before it's initialized, it will be "nil" by default

  * Global
    * runner files
    * only one "global" scope for the whole application

  * Ruby interprets code top to bottom
    * either learning code or executing code


#### What is scope?

 * Scope is what you have access to and where you have access to it.

  * Local Scope
  * Global Scope("top-level scope")
  * Class Scope (access to methods and instance variables and other classes and their methods)
  * Method scope ("sister scope")
  * Block scope(can call variable defined outside of block but variables defined inside blocked cannot be called outside of them)

#### for each of the following types of scope, what are the Ruby keywords that begin and end the scope.

 * Method Scope; def & end

 * Block Scope; do & end

 * Class Scope; class & corresponding end

 * Global Scope; anything outside of class, method, and block.

#### Extra Notes:

  * ruby
    ```attr_accessor :name
      def name(name = nil)
        unless name.nil?
          @name = name
          end
          return @name
          end
        end
      end
      ```
  * attr_readers are scope exports available globally outside of individual classes...to see the value.

  * discouraged use of global variables. in ruby all it is is a variable w/ a dollar sign before it. ie $a = 5
