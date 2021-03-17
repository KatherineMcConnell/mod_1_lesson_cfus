# Objects, Classes, and Instances

## Check for Understanding

#### Classes, instances, objects


  * What is a Class?

      A class is something that models state & behavior. There are superclasses too. But more on that later.

  * What is an Instance?

      An instance aka object is a concrete representation of a class. Aka one specific example of in a specific class. A class is like a blueprint for a house.

  * What is an Object?

      An object is an instance. Each instance has its own object id which is created in as a memory location in a local system. However, each time a new variable is set or changed/replaced, a new object id is set. So the instance is an object of the class. The actual house is an object or instance.

  * How are these three things alike/different?

      See above. A class is the blueprint, the instance is the house. The instance is aka object so an instance of a class is an object of a class.

      Classes are written in CamelCase.
      Objects/Instances in snake_case.

      class creation is used with a lower case class. And each class has it's own file.

      While objects are all instantiated in the runner.rb file I think. And the class files are required and loaded.


  * What code do you have to write to create a Class? What code do you have to write to create an instance?

    Class is CamelCase.
    Objects/Instances are snake_case.

    class Class
    end

    class = Class.new(arg, arg, etc)

  * What happens when a new instance is created?

    When a new instance is created it is "instantiated". It runs through the initialize method in the class file to be created with persisting attributes that the class has/is. ie the states. Initialize is only run once in an objects lifetime.


#### Attributes & Methods


  * What is an attribute?

    An attribute is denoted with the @ symbol in front of it and turning it into an 'instance variable' when it is set equal to something. Attributes are all initialized in the initialize method upon instantiation (creation). The attributes are the argument placeholder name associated to the instance variable. An attribute is a state of a class. NOT a behavior. Methods are behaviors.

    ie:
    ```
    class Dog

      def initialize(color, type)
      @type = type
      @color = color
    end
      ```

      @type is the attribute
      @type = type is the instance variable
      def initialize(color, type) are the placeholder arguments.

      Convention is to set them with names that are similar to show their connection. Also one can set an attribute value equal to an empty hash, array, or boolean and not include this in the arguments. These are considered default values.

  * How can we recognize an attribute?

      Denoted with @symbol before it.

  * What is a method? How do we write methods?

    A method is a behavior of a class. Methods can be attr_reader automatic methods of attributes or custom methods.

    Custom methods be command or query methods while attr_readers are **generally** query methods.

    Custom Method written:
    ```
    class Dog
      attr_reader :type,
                  :color

      def initialize(color, type)
      @type = type
      @color = color
    end

    Def method_name(any_args, etc)
      bark
    end
      ```
    The attr_readers are query methods. And the custom behavior methods are below the initialize method. The initialize method is run only once in an objects lifetime.

  * What are parameters? How do we add parameters to methods?

    Parameters are placeholder name that represent arguments given in the instantiation of a new object. A add parameters to methods by putting them directly after on the same line where we define the method


  * What is a return value? How do you know what the return value of a method is? Do all methods have return values?

    A return value denoted by => in pry. There is only one return value per method applied on an object.

    Query methods do not have return values you can see except for in pry. All methods do have return values.

    **If you are struggling a bit to answer any of these, take some time after this lesson to google or talk with a classmate. If you feel absolutely lost in these, set up a time to pair with a Mod2 student/mentor/instructor.**

    **I am stuggling specifically with table_print gem trying to print out the tables in the solo practice**

    **?? Attr_readers: how do they turn to methods? What are they taking from??**
