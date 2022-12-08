# learn-ruby

# Introduction to Ruby

**Ruby Variables**

myVar = 48

**Put and print command**

print "Hello" \
puts "This is written in a new line" \
print "Still printing" 

**Code comments in Ruby**

Single line comments start with a #.  \
Multi line comments start with =begin and end with =end.

Example: \
\# I am a single line comment.

=begin \
I am a multi line comment. \
I can take as many lines as needed. \
=end


**Numeric data types in Ruby**

\# Integer value \
x = 1

\# Float value \
y = 1.2

**Arithmetic operations in Ruby**

print 2*3 \
\# Multiplication: output 6 

print 2**3 \
\# Exponentiation: output 8 

print 16%9 \
\# Modulo: output 7

**Ruby Object Methods**

var = "codecademy"

\# Method to get the length of a string \
print var.length # 10

\# Method to get the string reversed \
print var.reverse # ymedacedoc

\# Method to conver all letters to uppercase \
print var.upcase # CODECADEMY

**Strings in Ruby**

\# String 1 \
s1 = 'I am a single string!'

\# String 2 \
s2 = "I am a double string!"

**Boolean Data Types in Ruby**

\# Boolean true variable \
year2019 = true

\# Boolean false variable \
year2018 = false

**Ruby .upcase and .downcase Methods**

puts "codecademy".upcase \
\# CODECADEMY

puts "Codecademy".downcase \
\# codecademy

**Ruby string interpolation**

age = 30

print "Hi, my name is Cody, and I am #{age} years old" \
\# "Hi, my name is Cody, and I am 30 years old"

# Control Flow in Ruby

**elsif Statements in Ruby**

print "enter a number: " \
num = gets.chomp \
num =  num.to_i; 

if num == 5 \
  print "number is 5" \
elsif num == 10 \
  print "number is 10" \
elsif num == 11 \
  print "number is 11" \
else \
  print "number is something other than 5, 10, or 11" \
end

**Ruby not Operator**

The ! (not) operator in Ruby flips a boolean value. If a value is true then applying ! to the value changes it to false and vice versa.

**Else statement in Ruby.**

if number > 50 \
  print "number is greater than 50" \
else \
  print "number is not greater than 50" \
end  
  
**Comparison operators in Ruby.**

The following comparison or relational operators are used in Ruby to compare values.

\> - greater than; \
\< - less than; \
\>= - greater than or equal to;  \
\<= - less than or equal to;  \
\== - equal to

**Or operator in Ruby.**

grade1 = 50 \
grade2 = 30 \
grade3 = 80

if grade1 > grade2 || grade1 > grade3 \
  puts "Grade 1 is not the lowest score!" \
end

**if Statement in Ruby**

number = 10 \
if number == 10 \
  puts "Your condition was true!" \
end

**And operator in Ruby.**

if score1 > score2 && score1 > score3 \
  print "Score 1 is the greatest in value." \
else \
  print "Score 1 is not the greatest in value." \
end

**Unless statement in Ruby.**

\#This construct requires a "number" variable to be less than 10 in order to execute: \
print "Enter a number" \
number = gets.to_i \
unless number > 10 \
  puts "number is less than 10." \
end

# Looping with Ruby

**Ruby Assignment Operators**

Assignment operators in Ruby are used to assign or update values to variables. The most common assignment operator is = but others also exist, like +=, -=, *= and /=.

**Ruby each Method**

To iterate over an array in Ruby, use the .each method. It is preferred over a for loop as it is guaranteed to iterate through each element of an array.

**Ruby “next” Keyword**

for i in 1..10 \
  next if i % 2 == 0 \
  puts i \
end

#In this example, the next keyword along with a shorthand if statement is used to skip over the even numbers in the sequence.
  
\# Output: \
\# 1 \
\# 3 \
\# 5 \
\# 7 \
\# 9

**Ruby while Loop**

**Ruby times Method**


5.times { puts ""Codecademy"" }

\# Output:  \
\# Codecademy \
\# Codecademy \
\# Codecademy \
\# Codecademy \
\# Codecademy

**Ruby Range**

**Ruby loop**

**Ruby until Loop**

**Ruby for Loop**

# Arrays and Hashes

**Ruby Hash**

profile = { \
  "name" => "Magnus", \
  "profession" => "chess player", \
  "ranking" => 1, \
  "grandmaster?" => true \
}

/# "name", "profession", "ranking", and "grandmaster?" are the keys. "Magnus", "chess player", 1 and true are the values.

puts profile["name"] \# => Magnus

**Ruby Array**

numbers = [1, 2, 3, 4, 5] \
\#An array of Integers

words = ["See", "Spot", "run"] \
\#An array of Strings

mixed = ["hello", 5, true, 3.0] \
\#An array with a String, Integer, Boolean, and Float

empty = [] \
\#An empty array

**Ruby Hash New**

\#Creating a hash through literal notation: \
lunch = { \
  "protein" => "chicken", \
  "greens" => "lettuce", \
  "organic?" => true \
}

\#Creating a hash through Hash.new \
lunch = Hash.new \
puts lunch # => {}

**Ruby Hash Bracket Notation Adding Pairs**

\#Bracket notation applies to any hash, regardless of how it was initialized \
teammates = Hash.new \
teammates["forward"] = "Messi" 

salary = { \
  "starting" => 40000 \
} \
salary["mid-level"] = 60000

**Ruby Multidimensional Arrays**

multi_array = [[0,1,2,3],[4.5, true, "hi"]]

\# Accessing the array at index 1 \
puts multi_array[1] \# => [4.5, true, "hi"]

\# Accessing the element at index 0 within the array at index 1 \
puts multi_array[1][0] \# => 4.5

**Ruby Array Index**

example = ["Car", "Boar", 45, 9.9, true]

\#For an array named `example`, you can retrieve an item of a particular index by referencing its index.

puts example[2] \# => 45 \
puts example[0] \# => Car

**Ruby Method .Each**

\#In this example, the each method iterates over every color in the colors array and prints it to the console.

colors = ["red", "blue", "green", "yellow"]

colors.each { |color| puts color } \
\#Output \
\#red \
\#blue \
\#green \
\#yellow

\#When iterating over hashes, two placeholder variables are needed to represent each key/value pair.

polygons = { \
  "pentagon" => 5, \
  "hexagon" => 6, \
  "nonagon" => 9 \
}

polygons.each do |shape, sides| \
  puts "A \#{shape} has \#{sides} sides." \
end

\#Output \
\#A pentagon has 5 sides. \
\#A hexagon has 6 sides. \
\#A nonagon has 9 sides.

**Ruby Hash Bracket Notation Value**

my_love = { \
  "dog" => "Keanu", \
  "breed" => "Shiba Inu", \
  "age_in_years" => 1, \
}

puts my_love["breed"] \# => Shiba Inu

# Blocks and Sorting

**Ruby Combined Comparison Operator**

puts "Keanu" <=> "Adrianna" # The first letters of each word are compared in ASCII order and since "K" comes after "A", 1 is printed.

puts 1 <=> 2 \# -1

puts 3 <=> 3 \# 0

\#<=> can also be used inside of a block and to sort values in descending order: \
my_array = [3, 0, 8, 7, 1, 6, 5, 9, 4] \
my_array.sort! { |first_num, second_num| second_num <=> first_num } \
print my_array \
\#Output => [9, 8, 7, 6, 5, 4, 3, 1, 0]

**Ruby Method Splat**

\#The * preceding the parameter "clubs" allows for multiple arguments to be passed into the method when you actually call it. \
def extra_curriculars(*clubs) \
  clubs.each { |club| puts "After school, I'm involved with #{club}" } \
end

extra_curriculars("chess club", "gymnastics", "anime club", "library services")

\#Output \
\#After school, I'm involved with chess club \
\#After school, I'm involved with gymnastics \
\#After school, I'm involved with anime club \
\#After school, I'm involved with library services

**Ruby Block Parameter**

\# The block, {|i| puts i}, is passed the current array item each time it is evaluated. This block prints the item. \
[1, 2, 3, 4, 5].each { |i| puts i }

**Ruby Return**

def generous_tip(bill) \
  return bill * (0.25) \
end

generous_tip(100) # 25

\#In this example, the generous_tip method is returning the product of bill and 0.25. In order to see that value, a "puts" or "print" can be added before the method call.

**Ruby Sort Method**

my_array = [3, 4, 8, 7, 1, 6, 5, 9, 2] \
my_array.sort! \
\#Attaching an ! to the end of .sort or any other Ruby method modifies the original array. \
print my_array \
\# => [1, 2, 3, 4, 5, 6, 7, 8, 9] \
\#If you didn't use !, print my_array returns the original array.

**Ruby Method Parameters & Arguments**

def square(num) \# num is the parameter \
  puts num ** 2 \
end

square(5) \#5 is the argument \
\#Output => 25

**Ruby method**

def greeting \
  puts "Hello world!" \
end

\#In this example, the first line or header contains the keyword "def" and the method name. puts "Hello world!" is within the body of the method, which describes the certain task that the method carries out. It is also indented two spaces by convention. Following the body, the method ends with the end keyword.

**Ruby Block**

2.times do \
  puts "I'm a code block!" \
end  

\#Output \
\#I'm a code block! \
\#I'm a code block!

3.times { puts "So am I!" }

\#Output \
\#"So am I!" \
\#"So am I!" \
\#"So am I!"

****
****
****
****
****

****
****
****
****
****
****
****
****
****
****

****
****
****
****
****
****
****
****
****
****

****
****
****
****
****
****
****
****
****
****

****
****
****
****
****
****
****
****
****
****

****
****
****
****
****
****
****
****
****
****

****
****
****
****
****
