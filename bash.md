# Introduction of bash
##### what is bash??
**Bash = Bourne Again Shell**
- It is a shell, that used to interact with your kernel.
##### What is Script?
- **Script is a file that contains shell commands in a simple and clear algorithm.**
- The original is sh - Bourne shell
## Uses of bash
● **Script development**
● **Automating tasks**
● **Simplifying your linux ability**
● **Developing hacking scripts.**
#### File Extension of bash
● Bash files can have “.sh” extension but you can have it without ‘.sh’ too
● The file have to have executable Permissions.
● You can use any text editors u need: VIM,nano,VScode,gedit,cherrytree…
#### Displaying output
**● To start Every bash scripts use shebang.**
                ○#! /bin/bash
                ○ #! /bin/sh
**● To display outputs on bash you just do**
             ○ echo “YOUR TEXT HERE"
**● To run your project you can do:**
    ○  /bin/bash hello.sh
    ○ ./hello.sh -> need x
    ○ hello -> need x
- **To display out put you can write echo "*your text*"**
            echo "Good Morning coders.."
#### Varible 
● Bash Variables are same with python variables, with some exceptions.
● Syntax:
○ VARIABLE_NAME=value
● Exceptions:
- *NO Space between the equal sign ( = )*
■ NAME = “Yared” => ERROR
■ NAME=”Yared” => Correct.
■ Never Start with Numbers
■ USE double quotes only.
- To use the variable we will use dollar sign( $ ) before the Variable name
- If you want to display the variable sticked with other text use ${VARIABLE_NAME}
● **Bash Variables are string by default.**
 - set used to assign values positional paremeters
 ###### sayntax
 - `set yared mistre josi dagim `
            set yared josi mister dagi
            echo $1 $2  # it index start with 1
 - To call the set we can use 
 -  echo $1 $2  # it index start with 1
 #### System variable
 - **system variables are varible that declard by the system this are:-**
 - `echo $BASH # `
 - `echo $BASH_VERSION`
 - `echo $PWD`
 - `echo $HOME`
 - `echo $PATH`
##### Variables & Data Types
● As we saw, the previous method they create strings only.
● So to create other data types we use declare.
● Arrays
- a) Arrays are lists or tuples on python.
- b) Syntax:
- i) var=(“list1” “list2” “list3” “list4)
- ii) TO display echo
- (1) ${var[0]}
- iii) To get all the elements
- (1) ${var[@]}
- i) To get the indexes
- (1) ${!var[@]}
- ii) To get the length
- (1) ${#var[@]}
- iii) To add element to the array
- (1) var[4]=”list5”
- iv) To remove from the array
- (1) unset var[3]
#### Bash Input
-  On bash we have 2 methods to accept input
- 1. Read function
- 2. Arguments
- 1) Bash read
- ● Read used to accept inputs while the script is running.
- ● Syntax:
- ○ read -p “Text To Display” var
- ○ read -sp “Password: ” var => used to accept hidden texts like password.
- ○ read -a var => for accepting arrays(lists)
- 2) **Arguments**
- ● These helps to get input before the script starts
- ● Syntax:
- ○ Just use $0-$9 while you want to work with the input
#### Comments
- On bash the comments are
- For multi line comment we start with
- <<COMMENTS
- Sfasf
- Sfa
- COMMENTS , we close with this
- Bash sleep
- ● Sleep used to make a good waiting on our script.
- ● Syntax:
- ○ sleep <number>s
##### Operation
- ● To do mathematical operations you have to do $(( expression ))
- ● we will use let keyword for assigning variable
- A) Arithmetic Operations
- a) Addition $(( a + b ))
- b) Subtraction $(( a - b ))
- c) Multiplication $(( a * b ))
- d) Division $(( a / b ))
- e) Exponential $(( a ** b ))
- f) Modulo $(( a % b ))
- #### B) Assignment Operations
- a) Increment “let a+= 3”
- b) Decrement “ let a-= 3”
- c) Multiply “ let a*= 3 “
- d) Divide “ let a/=3 “

#### C) Comparison operation
- Alphabetic comparison
- Greater Than => -gt
- Less Than => -lt
- Greater than and equals to => -ge
- Less than and equals too => -le
- Equal => -eq
- Not equal => -ne
- #### Sign comparison
● >
● <
● >=
● <=
● =
● !=

#### If else conditions
● Syntax:
○
● If you used [ condition ] => you will use alphabetic comparison
● But for strings you can use
- sign too
- If you used (( condition )) => you
- will use numeric comparison
- On bash we don't have indentation but
- if u finished writing the body you type
- “fi”

