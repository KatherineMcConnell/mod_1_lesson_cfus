# Intro to Testing

## Check for Understanding

#### What 2 directories should we have within our project directory?

 * A lib directory for class files. And a spec directory test files to accompany each class file.

 * ie: student_spec.rb & student.rb.

#### Rspec setup:

#### What do you have to require in a spec file?

  * You have to require the lib file in your spec file as well as rspec.

  * ie:
  require 'rspec'
  require '../lib/student'

#### What goes in the initial describe block?

  * The initial describe block has the class name. ie:
  describe Student do.
  
  * The tests inside this first block can test the instance of is initialized and attributes of the class.

  * describe blocks are describe the functionality of a group of tests ie 'describe instance methods' with a bunch of method tests under it.

  * typically you'll only see 2-3 describe blocks in a spec file

  * rspec -f d command will show all of the describe & it block text created.

#### What is the syntax for a rspec spec?

  * Uses wors "describe" and "it" so we can express concepts like a conversation.

  * The syntax for the rspec spec is:

  ```
  describe **class** do
      describe '**#actual_method_name**' do
        world aka setup
        it '**description of method/return value**' do
          expect(class/class.method).to be or to eq (etc .to methods of rspec see documentation)
        end
      end
  end
  ```

#### Name 3 **.to methods** you learned about today & describe their syntax.

 * See this documentation which will help in the future.

 https://rubydoc.info/gems/rspec-expectations

#### Other:

  * files should be run from the project root directory. To see only a specific spec file use the file path.

  * if a repo created by someone else running a different version a ruby may need to be run using bundle exec rspec

  * Spiking is used when you don't understanding how to figure out how to write a test, logic of it, where to even start. You can play with code until you better understand. Then delete the Spike code. Write your test. Pass your test.
