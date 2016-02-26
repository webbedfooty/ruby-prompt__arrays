Testing by Patrick

---
title: Arrays
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is an Array?

An Array is a data object that stores a list of values in a particular order; aka list in other program languages.


# What are some examples of information that would be Arrays as opposed to some other data type?

"Arrays are distinguished from lists in that arrays allow random access, while lists only allow sequential access" as said here:
https://en.wikipedia.org/wiki/Array_data_type


# What is one way, using Ruby, to retrieve the 6th element in an Array? How about the 8th element? What happens if you try to retrieve the value of the _9999th_ element (or some element that doesn't exist in the array)?

puts array[5] # the position you want = element -1
puts array[7] # put a different way, the element = position +1
If there isn't an element in the X position, it will simply return a blank space there


# The previous question asks about finding, for example, the 6th element in an Array. Is it possible to find the **-6th** (Notice the negative symbol!) element in an Array? What does that even mean?

Yes you can, assuming there are at least 6 elements in the array.
What it means is that it counts backward from the end of the array, going right to left as opposed to forward, left to right.


# How would you perform an operation on every element inside an Array?

Using the .each method
"The each method yields a reference to each element in the collection, rather than a reference to the element's numerical index in the array"


# How do you add elements to an Array?

You can either use the .push method or <<
array = [1, 2, 3, 4]
array.push(5)
  or
array << 5
Both ways adds the element at the end of the line
Another cumbersome way would be to + [5] to the array


# Given the Array `["Laura", "Fiona", "Tori"]`, how would you replace `"Fiona"` with `"Florence"` so that you end up with `["Laura", "Florence", "Tori"]`?

array[1] = "Florence"


# What do the methods `push`, `pop`, `shift`, and `unshift` do?

 .push adds an element to the end of the array
 .pop removes the last element of the array
 .shift removes the first element of the array
 .unshift prepends an element to the beginning of the array


# How do you determine how many elements are in an Array?

array.length


# How would you reverse the order of elements in an Array?

array.reverse


# How would you convert a String `"Sumeet Jain"` into an Array `["Sumeet", "Jain"]`? How about to `["S", "u", "m", "e", "e", "t", " ", "J", "a", "i", "n"]`? How would you convert the Array back into a String?

name = "Sumeet Jain"
array = name.split


array = []
name = "Sumeet Jain"
y = name.length
x = 0
while x != y
array[x] = name[x]
x = x + 1
end
puts array


## Question, how do you get it so that it adds in the double quotes and the comma separator as seen in part 1 of this question?

Answer to part 2 of this question is to add the line
puts array.join