# CONDITIONAL AND LOOPING STATEMENTS


## Conditional and Looping Statements in Python

## Conditional and looping statements are fundamental building blocks in Python, allowing you to control the flow of your programs.

## 1. Conditional Statements (if, elif, else)

## Conditional statements enable your program to make decisions based on whether certain conditions are true or false.

## 2. Looping Statements (for, while)

## Looping statements allow you to repeat a block of code multiple times.



### Exercise 1
##### Name your file: MonthNames.py
##### Write a program that reads an integer value between 1 and 12 from the user and prints output the corresponding month of the year.

### PROGRAM-1

d={1:"January",2:"February",3:"March",4:"April",5:"May",6:"June",7:"July",8:"August",9:"September",10:"October",11:"November",12:"December"}

s=int(input("Enter the number: "))

if 1<=s<=12:

    a=d.get(s)
    
    print("The month ",s," is",a)

### OUTPUT-1 

![image](https://github.com/user-attachments/assets/391d727b-0a47-4177-95c8-6d15e60ef702)


### Exercise 2
#### A certain cinema currently sells tickets for a full price of 6 pounds, but always sells tickets for half price to people who are less than 16 years old, and for a third of the price for people who are 60 years old or more.

### PROGRAM-2

age=int(input("Enter your age:"))

t=6

if age<16:

    ticket=t*(1/2)
    
    print(f"Your ticket costs £{ticket:.2f}")
    
elif age>60:

    ticket=t*(1/3)
    
    print(f"Your ticket costs £{ticket:.2f}")
    
else:

    ticket=t
    
    print(f"Your ticket costs £{ticket:.2f}")


### OUTPUT-2 

![image](https://github.com/user-attachments/assets/c43e51c1-551a-452d-9a24-c11b9598408d)



### Exercise 3

#### Name your file: BodyMassIndex.py

#### Write a program to calculate your BMI and give weight status. Body Mass Index (BMI) is an internationally used measurement to check if you are a healthy weight for your height.The metric BMI formula accepts weight in kilograms and height in meters:
#### BMI= weight(kg)/height2(m2)
#### BMI Weight Status Categories table
#### BMI range - kg/m2 Category
#### Below 18.5 Underweight
#### 18.5 -24.9 Normal
#### 25 - 29.9 Overweight
#### 30 & Above Obese

### PROGRAM-3

w=int(input("Enter your weight in kg :"))

h=float(input("Enter your height in m :"))

bmi=round(w/(h*h),2)

print("Your BMI is:",bmi)

if 18.5<=bmi<=24.9:

    print("You are in normal range")
    
elif 25<=bmi<=29.9:

      print("You are in overweight range")
      
elif bmi<18.5:

 print("You are in underweight range")
 
else:

 print("You are in obese range")

 
### OUTPUT-3

![image](https://github.com/user-attachments/assets/86f6a8b9-2a6d-40bd-8769-b4c81763ca72)



### Exercise 4

#### Write a Python program to receive 3 numbers from the user and print the greatest among them.

### PROGRAM-4

n1=int(input("Enter the first number"))

n2=int(input("Enter the second number"))

n3=int(input("Enter the third number"))

if n2<n1>n3:

    print(n1,"is the greatest number")
    
elif n1<n2>n3:

    print(n2,"is the greatest number")
    
else:

    print(n3,"is the greatest number")



### OUTPUT-4

![image](https://github.com/user-attachments/assets/f374f900-806e-4693-bdb2-e10d674ade50)


### Exercise 5

#### Find the factorial of a given number using loops(note the number is received from the user)

### PROGRAM-5

n=int(input("Enter the positive number whose factorial is to be found"))

if n<0:

    print("Factorial is not defined for negative numbers")
    
elif n==0:

    print("Factorial is not defined for zero")
    
else:

    fact=1
    
    i=1
    
    while i<=n:
    
        fact=fact*i
        
        i=i+1
     
    
print (fact)


### OUTPUT-5

![image](https://github.com/user-attachments/assets/e3ae62a7-1ee9-47b5-aee6-3758b12def19)


### Exercise 6

#### Reverse a number using while loop


### PROGRAM-6

n=int(input("Enter the number to be reversed"))

reverse=0

while n>0:

    digit=n%10
    
    reverse=reverse*10+digit
    
    n//=10


print("The reverse of",n,"is:",reverse)


### OUTPUT-6

![image](https://github.com/user-attachments/assets/97a76347-9c5c-429c-805b-6aa4042aa663)


### Exercise 7

#### Finding the multiples of a number using loop

### PROGRAM-7

n=int(input("Enter the number whose multiple is to be found : "))

c=int(input("\nEnter the count of multiples you may need. The multiples starts by multiplying your entered digit from 1 till the count you may enter : "))

print("\nThe ",c,"multiples of the number ",n,"are:")


for i in range(1,c+1):

    multiple=n*i
    
    print(multiple)
    


### OUTPUT-7

![image](https://github.com/user-attachments/assets/97b729f5-292a-4efc-8868-6779f75c8f24)


### Exercise 8

#### Write a program to print the inputted value as it is and break the loop if the value is 'done'.


### PROGRAM-8


while True:

    n=input("Enter the value to be printed: ")
    
    
    if n=="done":
    
        print(n)
        
        break
        
    else:
    
        print(n)



### OUTPUT-8 

![image](https://github.com/user-attachments/assets/e08d2556-f8ab-4758-8d5d-5c6a901be27d)


### Exercise 9

#### Write a program that prints the numbers from 1 to 10. But for multiples of three print "Fizz" instead of the number and for the multiple of five print "Buzz". For numbers which are multiples of both three and five print "FizzBuzz"


### PROGRAM-9

for n in range(1,11):

    if n%3==0:
    
        print("Fizz")
        
    elif n%5==0:
    
        print("Buzz")
        
    elif n%3==0==n%5:
    
        print("FizzBuzz")
        
    else:
    
        print(n)



### OUTPUT-9

![image](https://github.com/user-attachments/assets/d462016e-cd3b-4250-80ef-09c28474d836)


### Exercise 10

#### Write a program to print the following pattern:
##### 5 4 3 2 1
##### 4 3 2 1
##### 3 2 1
##### 2 1
##### 1


### PROGRAM-10

rows=5

for i in range(rows,0,-1):

    
    for j in range(i,0,-1):
    
        print(j,end=" ")
        
    print("\n")


### OUTPUT-10

![image](https://github.com/user-attachments/assets/a7f8ebc0-165a-4268-aa65-f53c9953b10e)





        




