## Experiment [4]: [Bash Scripting]
### Name:Shashwat Agrawal, Roll No.: 590029107, Date: 2025-09-04
### AIM: 
* [To Learn Basics of Bash Scripting.]

### Requirements:
* [Any Linux Distro, any kind of text editor (vs code, vim, notepad, nano, etc)]

### Theory: 
* [Learning the basics of bash scripting.]

## Procedure & Observations

## Exercise 1: [Hello World Script]

## Task Statement: 
* [Basic Usage of Shell Scripts]

## Explanation: 
* [Writing Begginer level Shell Scripts]

## Command(s):
```
#!/bin/bash
echo "Hello, World!"

```

#### Output:
<img width="958" height="411" alt="Screenshot 2025-11-06 222402" src="https://github.com/user-attachments/assets/d697dc60-a5e4-48c6-8b13-efcd794835a4" />



## Exercise 2: [Personalized Greeting Script]

## Task Statement: 
* [Basic Shell Script to callout user defined function.]

## Explanation: 
* [This Shell script will take input from user and store it in a variable and then call the variable which will output the stored value.]

## Command(s):
```
#!/bin/bash
echo "What is your name?"
read name
echo "Hello, $name! Welcome to Shell Scripting."

``` 

## output
<img width="949" height="464" alt="Screenshot 2025-11-06 222531" src="https://github.com/user-attachments/assets/90d8570c-2d15-4a01-9476-c983e6f93221" />



## Exercise 3: [Arithmetic Operations in Shell Scripting]

## Task Statement:
* [Using Basic Arithmetic Operations in Shell Scripts]

## Command(s):
```

#!/bin/bash
echo "Enter first number: "
read num1
echo "Enter second number: "
read num2

echo "Addition: $((num1 + num2))"
echo "Subtraction: $((num1 - num2))"
echo "Multiplication: $((num1 * num2))"
echo "Division: $((num1 / num2))"

```

## Output:
<img width="953" height="485" alt="Screenshot 2025-11-06 222845" src="https://github.com/user-attachments/assets/593a002c-014e-4a4d-926c-c4b155db4362" />


## Exercise 4:
* [Voting Eligibility]

## Task Statement:
* [Using Conditionals in Shell script ]

## Command(s):
```
#!/bin/bash
echo "What is your age?"
read age
if [ $age -ge 18 ]; then
    
    echo "You are eligible to vote!"
    
else 
    echo "You are not eligible to vote!"

fi

```

## Output:
<img width="951" height="476" alt="Screenshot 2025-11-06 223231" src="https://github.com/user-attachments/assets/54d04d8c-92f4-41fd-8c83-0298e14643e6" />


## Result
* The Exercises were successfully completed for Basic Shell Scripting
