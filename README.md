# learn-python-part1

Click the snake to see the code and explanation about my code
<!-- 
<details><summary>:snake: </summary>
<p>

```python
   
```
</p>
</details>


*******************************************
-->
<details><summary>:snake: Nested loop</summary>
<p>

```python
for i in range(3):
	for k in range(3):
		print(f"{i}, {k}") #it will print : row : 0 1 2, colom : 0 1 2

print()

count = 0
for i in range(3):
	for k in range(2):
		count += 1

print(count) # 6

print()
for i in range(2):
	print(i)
	for k in range(3):
		print(k)
	print("***") # it will print 0 3X in first colom , second colom 0 1 2, *** then 1 3x, second colom 0 1 2, then ***

print()
for i in range(1,4):
	for k in range(i):
		print(f"{i},{k}") #ffirst colom: 1 3x, 2 3X, 3 3X, second colom : 0 , 1 1, 2 2 2

   
```
</p>
</details>


<details><summary>:snake: List</summary>
<p>

```python
animals = ["dog","cat","fish","bird"]
print(animals)
print(animals[3])
animals[2] = "hedgehog"
print(animals)
#animals[4] = "camel"
print(animals)
animals.append("whale")
print(animals)
animals.insert(1,"snake")
print(animals)
animals.extend(["camel","shark"])
print(animals)

animals.append(["bug","lion"])
print(animals)

animals.append("dog")
print(animals)

animals.pop(1)
print(animals)

animals.remove("camel")
print(animals)


animals.remove("dog")
print(animals)
print(len(animals))

for animal in animals:
	print(animal)

   
```
</p>
</details>


<details><summary>:snake: Guessing game </summary>
<p>

```python

number = 0
while number !=2:
	print("guess a number: ")
	number = int(input())


	if number == 2:
		print("you win")
		
	else:
		print("try again:  ")	

# 5 attempt guess numbers

count = 0
while True:
	count +=1
	
	print("guess a number: ")
	number = int(input())


	if number == 2:
		print("you win")
		break
	elif count == 5:
		print("you lose!")
		break
	else:
		print("try again")	
 
```
</p>
</details>

<details><summary>:snake: Loop (for, infinite and while)</summary>
<p>

```python

a=0
while a<=3:
	print(a)
	a=a+1
a = 10
while a>=0:
	print(a)
	a=a-1
print("Blastoff!")
print(a)

#infinite loop, to break it with ctr-c

c=0
while c<5:
	print(c)


d=0
while True:
	print(d)
	if d==2:
		break
	d=d+1

for i in range(4):
	print(i)

for i in range(10,21):
	print(i)

print()

for i in range(21):
	if i%2 == 0:
		print(i)

print()

for i in range(10,-1,-1):
	print(i)
print("Blassoff!")

   
```
</p>
</details>


<details><summary>:snake: Company pricing </summary>
<p>

```python
   #9 company pricing exercise solution2

print("Company pricing plan: ")
print(" first 500 is 10 cent each")
print(" next 500 is 5 cent each")
print(" anything more is 1 cent each")

#company pricing exercise solution2

print("Company pricing plan: ")
print(" first 500 is 10 cent each")
print(" next 500 is 5 cent each")
print(" anything more is 1 cent each")

print(" how many you want to buy: ")
order = int(input())
orderA = order * 10
orderB = 500*10 + (order-500)*5
orderC = 500*10 + 500*5 + order-1000

if order <=500:
	print(f"your order is {order}, your total is: ${(orderA/100)} ")
elif 500<order<=1000:
	print(f"your order is {order}, your total is: ${(orderB/100)} ")
else:
	print(f"your order is {order}, your total is: ${(orderC/100)} ")

print(" how many you want to buy: ")
order = int(input())

orderA = order * 10
orderB = 500*10 + (order-500)*5
orderC = 500*10 + 500*5 + order-1000
total = 0 
if order <=500:
	print(f"your order is {order}, your total is: ${(orderA/100)} ")
elif 500<order<=1000:
	print(f"your order is {order}, your total is: ${(orderB/100)} ")
else:
	print(f"your order is {order}, your total is: ${(orderC/100)} ")


```
</p>
</details>

<details><summary>:snake: Biggest number </summary>
<p>

```python
   # choose the biggest number with nesting 

print("enter a number: ")
numb1 = int(input())

print("enter a second number: ")
numb2 = int(input())

print("enter a third number: ")
numb3 = int(input())

if numb1<=numb2:
	if numb2<=numb3:
		print(f"the biggest number is {numb3}")
	elif numb2>=numb3:
		print(f"the biggest number is {numb2}")
elif numb1>=numb2:
	if numb1>=numb3:
		print(f"the biggest number is {numb1}")
	elif numb3>=numb1:
		print(f"the biggest number is {numb3}")


 # the biggest number with compound 

print("enter a number: ")
numb1 = int(input())

print("enter a second number: ")
numb2 = int(input())

print("enter a third number: ")
numb3 = int(input())


if numb1<=numb2<=numb3:
	print(f"the biggest number is {numb3}")
elif numb1<=numb2 and numb2>=numb3:
	print(f"the biggest number is {numb2}")
elif numb1>=numb2 and numb1>=numb3:
	print(f"the biggest number is {numb1}")
elif numb1>=numb2 and numb3>=numb1:
	print(f"the biggest number is {numb3}")


 # the biggest number just with if

print("enter a number: ")
numb1 = int(input())

print("enter a second number: ")
numb2 = int(input())

print("enter a third number: ")
numb3 = int(input())

if numb1>=numb2 and numb1>=numb3:
	print(f"the biggest number is {numb1}")
if numb2>=numb1 and numb2>=numb3:
	print(f"the biggest number is {numb2}")
if numb3>=numb1 and numb3>=numb2:
	print(f"the biggest number is {numb3}")

```
</p>
</details>

<details><summary>:snake: If statement practices</summary>
<p>

```python
#
print(" what is your fav programming language: ")
language = input()
if language == "Python" or language == "python":
	print("yay")
elif language == "Java" or language == "java":
	print(" I like that one too")
elif language == "Bash" or language == "bash":
	print("You most like LINUX")
else:
	print("I don't know that one")

# 4 Traffic light exercise

print("what light is on now: ")
light = input()
if light =="red":
	print("you have to stop now")
elif light == "yellow":
	print("please prepare to stop")
else:
	print("you can go now")

# 5 absolute number exercise

print ("enter a number : ")
number = int(input())
if number >=0:
	print(f"your  number is {number} ")
else:
	print(f"your absolute number is {abs(number)}")
'''
#2 square or rectangle exercise
'''
print(" enter the width :")
width = int(input())
print(" enter the length: ")
length = int( input())
if width == length:
	print("you make a square")
else:
	print("you make a rectangle")

#****even or odd number exercise 

print ("enter a number: ")
number = int(input())
if number % 2 == 0:
	print("your number is even number")
else:
	print("your number is odd number")

#company pricing exercise

print("Company pricing plan: ")
print(" first 500 is 10 cent each")
print(" next 500 is 5 cent each")
print(" anything more is 1 cent each")

print(" how many you want to buy: ")
order = int(input())
if order <= 500:
	print(f"your order is {order}, your total is: {order*10} cents")
elif 500<order<=1000:
	print(f"your order is {order}, your total is: {500*10 + (order-500)*5} cents")
else:
	print(f"your order is {order}, your total is: {(500*10 + (order-500)*5)+(order-1000)*1} cents")


# 1 what does each piece of the following code produce?

a = 1
b = 2
c = 3
if a < b:
	print("Alfa")
else:
	print("Bravo")
print("Charlie")
 
if b < c:
	print("Delta")
else:
	print("Echo")
	print("Foxtrot")
if a > b:
	print("Golf")
elif c > b:
	print("Hotel")
else:
	print("India")
if b > a:
	print("Juliet")
if a > c:
	print("Kilo")
if b > c:
	print("Lima")
else:
	print("Mike")


'''
It will print:
Alfa
Charlie
Delta
Hotel
Juliet
Mike
'''

# 3 print out the biggest number

print("Enter a first number: ")
numberA = int(input())
print("Enter a second number: ")
numberB = int(input())

if numberA > numberB:
	print(f"your biggest number is {numberA}")
if numberB > numberA:
	print(f"your biggest number is {numberB}")


# 6 Convert to letter grade

print("enter your number grade")
grade = int(input())

if grade >= 100:
	print(" You get an A+")
elif 90 <= grade <= 99:
	print("You get an A")
elif 80 <= grade <= 89:
	print("You get a B")
elif 70 <= grade <= 79:
	print("You get a C")
elif 60 <= grade <= 69:
	print("You get a D")
else:
	print("you get a F")


#7 ask two number 

print("Enter first number: ")
first = int(input())
print("Enter second number: ")
second = int(input())

if first%2 == 0:
	print(first * second)
elif first < 0:
	print(first + second)
elif second > 0:
	print(first**second)
else:
	 print("Can't do anything with these numbers")



#8 temperature 

print("do you prefer temperature in 'F' or 'C' ?")
temp = str(input())
print("what is the temperature now: ")
deg = int(input())

if temp == "C":
	print(f"Your temperature in F is: {int(deg * (9 / 5) + 32)}")
elif temp == "F":
	print(f"Your temperature in C is: {int((deg-32) * 5 / 9)}")



# ask two number and the sum more than 20

print("enter a number: ")
numb1 = int(input())
print("enter a second number: ")
numb2 = int(input())
total = numb1 + numb2
if total <20: 
	print("enter a third number: ")
	numb3 = int(input())
	total +=numb3
	print(f" your total number is: {total}")
	if total <20:
		print("enter a fourth number: ")
		numb4 = int(input())
		total += numb4
		if total <20:
			print(f" your total number is: {total}, it's still under 20")
		
		else:
			print(f"your sum number minus 5 is: {total-5}")
	else:
		print(f"your sum number minus 5 is: {total-5}")

else:
	print(f"your sum number minus 5 is: {total-5}")
   
```
</p>
</details>

<details><summary>:snake:If statements </summary>
<p>

```python
c = 0
if c > 0: 
	print("positive")
elif c < 0:
	print("negative")
else:
	print("Neither")   
```
</p>
</details>


<details><summary>:snake: User input</summary>
<p>

```python
'''print("enter an animal")
#animal = input()
print (f"I like {animal} too")
'''

print("what is your name :  ")
name = input()
print(f"Hello, {name} ")
print("what is your age:  ")
age = input()
age = int(age)
print(f"You are {age} years old.")
age = age - 10
print(f"Magically you are now {age} year old")
   
```
</p>
</details>

<details><summary>:snake: Variables </summary>
<p>

```python
fruit = "apple"
#Creating a variable called  with text apple inside of it
animal = "dog"
print(fruit)

print("I have a ")
print(animal)


print("I have a " + animal + " eating  an "+ fruit)

print(f"I have a {animal} eating  an {fruit}")

animal = "cat"
print(f"I have a {animal} eating  an {fruit}")

second_animal=animal
animal = "fish"
print (f"My animals are {animal} and {second_animal}")
# prediction out : My animals are fish and dog
   
```
</p>
</details>


<details><summary>:snake: Hello world </summary>
<p>

```python
   print("Hello world")
```
</p>
</details>
