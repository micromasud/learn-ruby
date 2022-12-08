# learn-ruby

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
