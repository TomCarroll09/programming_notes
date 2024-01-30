``` lua
Local var = "value"
```

Declares a local variable called var.

----

``` lua
string.lower()
```
Changes a strings capitalization to lower case

----

``` lua
string.upper()
```
Changes a string's capitalization to uppercase.

----

``` lua
string.len()
```

Calculates the lenght of a string. the same as #"string".

----

``` lua
local num1, num2, num3 = 12, 34, 65
```
Declares multiple variables at once.

----
``` lua
tostring()
```

Converts a number to a string

----

``` lua
tonumber()
```
Changes a string to a number

----

``` lua
type()
```
outputs the type of an object


# Math

If you want to control the order of maths sums, use bracets
``` lua
math.pi
```
outputs the value of pi

----

```lua
math.min()
```
chooses the lowest value in a collection.

----

``` lua
math.max()
```
chooses =the largestr number in a collection

----

``` lua
math.ceil()
```

Rounds up

----

``` lua
math.floor()
```
rounds down

----

``` lua
math.random()
```

generates a pseudo random number

----

``` lua
math.randomseed(os.time())
```
specifies a seed for the random number. this instance used the time from os.time.

----

# If statements

``` lua
if true then
	print("This was true")
end
```

An example of an if statement

----

list of operators:

``` lua
and
or
not
>
<
~=
==
```
Note that lua does not use \!= it uses ~=

----
``` lua
if true then
	print("true")
else
	print("false")
end
```
if/else statement in lua

-----

```
if true then
	print("It was true")
elseif false then
	print("IT was false")
else
	print("I dont know")
end
```
if/else/elseif statement in lua

----
```
local age = 19
local name = age > 18 and "mike" or "jeff"

print("Name")

```
if the age variabe is larger than 18 then it if mike, else it is jeff.

----

# Loops
----
``` lua
for i = 1, 10 do
	print(i)
end
```
for loop in lua

----

```
while true do
	print("This will never end!")
end

while true do
	print("this will end")
	break
end
```

an example of while loops

----

```lua
repeat
	print("Hello")
until condition
```

An example of a repeat loop, similar to a do loop in other langauges.

----

`
# user input

```
print("What is your name?")
local answer = io.read()
print("Name:", ans)

-- example 2
io.write("Enter your name: ")
local ans = io.read()

print("Name:", ans)

```

2 examples of input in lua, the first method prints, which appends a newline at the end. io.write() does not append a newline to the end.

----

# Tables

``` lua
local tbl = { "this is a string", 2, 8.9, true}
for i = 1, #tbl do
	print(tbl[i])
end
```
prints all of the parts of a table

----
``` lua
tbl = {"string", 45, false}
print(tbl[2])
print(tbl[1])
```
Prints specific parts of a table in this case, item 1 and 2

----
``` lua

table.insert(tableName, 2, "Value")
```
inserts an object into a table. the first argument is the table to insert to, the second the position, or if not specified the value, which is appended onto the end. the last argument is the value to insert

----

```lua
table.remove(tableName, 3)
```
removes the specified object from a table.

----
``` lua
local nums = {
	{ 1, 8, 3},
	{4, 8, 3},
	{7, 6, 7),
}

print(nums[1][2])
```

A multi dimenssional table. the example will print the value 8, from table 1.

----

``` lua
table.concat(tableName, " ")

```
outputs a table as a string, the second argument is what is put between individual values.

----
``` lua
local tbl = {
	name = "Tom",
	age = "14",
	planet = "earth"
}

print(tbl["name"]

```
Calls a named object from a table

----

# Functions

```lua
local function sayHello()
	print("Hello")
end

sayhello()
```
Declares a local function and calls it.

----
```lua
local function sayName(name)
	local name = name or "jack"
	print("hello " .. name .. "!")
end
sayName()
sayName("Harry")
```

sets a default value. to the argument.

----

# Working with files

``` lua
io.output("myFile.txt")
```
Creates a file called myFile.txt
NOTE: it will empty a file if it already exists

----
```lua
io.output("myFile.txt")

io.write("Hello, World!")

io.close()
```

Creates, writes to and closes a file

----
```lua
io.input("myFile.txt")
local fileData = io.read("*all")

print(fileData)
io.close()
```
opens a file for input, adds the contents of the file to the fileData variable and prints the output of the file. the fileData variable can be outputted after closing the file.

-----
```lua
local file = io.open("myFile.txt", "w")
if file ~= nil then
	file:write("Hello, there!")
	file:close()
else
	print("Could not open the file")
end
```
Writes to a file. if the file is nil, meaning it does not exist, the file will not be written to, and will print that the file couldnt be opened.

-----
```lua
local file = io.open("myFile.txt", "r")

if file ~= nil then
	print(file:read("*all"))
	file:close()
else
	print("Could not open the file")
end
```
prints the contents of a file

----
```lua
local file = io.open("Myfile.txt", "r")

if file ~= nil then
	print(file:read("*line"))
	print(file:read("*line"))
	print(file:read("*line"))
	file:close()
else
	print("Could not open the file")
end
```

Reads the file line by line.

----
```lua
local file = io.open("myFile.txt", "a")

if file ~= nil then
	file:write("Ayy, this is appended on to the file! ")
	file:close()
else
	print("The file could not be opened")
end
```
Appeneds some text on to the specified file. it will not start on a newline.

----

# external modules

----
``` lua

