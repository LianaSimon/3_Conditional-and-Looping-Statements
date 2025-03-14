# CONDITIONAL AND LOOPING STATEMENTS

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



