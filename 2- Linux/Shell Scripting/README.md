<h1 align="center"> Shell Scripting </h1>

### Shell
It is basically an interpreter which take user input as a command and then tell Kernal (which is basically the heart of OS) what to do according to the command entered.

Shell Scripting helps us to implement logic and bulk operations.

***Bash*** is one of the programming languages used to write shell scripts.

## Bash Syntax

### Variable

`variableName=value`

`name=Hammad`

`age=21`

*IMPORTANT THING* 
You have to give variable a name and then there is no space between variable name and *=* sign. Otherwise, there will be error.

### Reusing Variable

For reusing variable the given variable, you have to type dollar sign *$* before variable name

`ageAtGraduation=$((age+3))`

### Storing output of a command in a Variable

`varName=$(command)  ` For Example, `lsResult=$(ls test)` ***test is the name of the folder***

### Conditionals 

#### Syntax

``` 
    if [ condition ]
    then
        statement
    elif [ condition ]
    then
        statement
    else
        statement
    fi
```

### Taking input from outside

For this, you have to write `$1` `$2` so on. When you will write `varName=$1`. The first input on the termainal will be replaced with this `$1` and so on.

Suppose, you have two variables that are storing the input given in terminal but the user give three or more than three inputs, then the rest of inputs will be stored in `$*`
You can print then using 

`echo "Here are all the given inputs in terminal:  $*`

If you want to print them one by one, you can do it using ### Loops

### Syntax of For Loop

```
for var in $*
do 
  $var
done
```

### Syntax of While Loop

```
while [ condition ]
    do
        statement
    done
```


### Functions

### Syntax
```
function functionName() {
  statement
}
```
For calling function, you have to only type functionName

``` 
function a(){
    echo "Hey I am a Funciton"
}

a
```
This will print what is written inside the function










