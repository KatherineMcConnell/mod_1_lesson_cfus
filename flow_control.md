# Flow Control

## Check for Understanding

#### Comparison Operators: All return Booleans

#### Boolean - something that is either true or false

#### Comparison Examples:

  * >
  * >=
  * <
  * <= aka hungry hippos hate me & always will
  * != aka not equal to
  * == aka equal to
  * || && aka or and (&& is pronounced double ampersand)

  *****************

  * Most specific case up top. The order in which conditionals are stuctured are really important.

  * ???? So on i-miss-eating-out... would you #announce closing time. Would you want the PM calc first or AM. It doesn't seem to matter but? Convention.

  * PEMDAS Order of Operations

#### What will the following code print to the screen?

```
  play_again = true
  lives = 3

  if lives == 0
    puts "You Lose!"
  elsif !play_again
    puts "Game Over!"
  elsif play_again && lives > 0
    puts "Welcome back!"
  else
    puts "invalid input"
  end
```
"Welcome back!"
*******************

What values would play_again and lives need to be assigned to in order to print each of the following to your terminal:

  * “You Lose!” if Lives = 0
  * “Game Over!” if Play_Again = false
  * “Welcome back!” if play_again = true and lives is greater than 0
  * “Invalid input if any of the above conditions are not met.

#### Loops

a set of instructions that is executed until a condition is met.

Using times, while, until and loop, print “Beetlejuice” to the terminal 3 times. 🐝

  * Times

  ```ruby
  3.times do
    puts "Beetlejuice"
  end
  ```

  * While runs while condition is true

  ```ruby
  while num <= 3 do
    num = num + 1
    puts "Beetlejuice"
  end
  ```

  * Until runs until condition is false

  ```ruby
  puts "until below"
  num = 0
  until num == 3 do
    num = num + 1
    puts "Beettlejuice"
  end
  ```

  * Loop do runs forever until used break

  ```ruby
  puts "loop do below"
  num = 0
  loop do
    num += 1
    if num < 4
      puts "Beetlejuice"
    end
  end
  ```
