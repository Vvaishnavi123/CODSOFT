# CODSOFT
#internship1
#scientific calculator
def addition(a,b):
    return a+b
def sub(a,b):
    return a-b
def mul(a,b):
    return a*b
def div(a,b):
    return a/b
print("select operations:")
print("1.Addition\n","2.sub\n","3.mul\n","4.div\n")
operation=int(input("enter your choice:1/2/3/4=="))
a=int(input("enter value of a:"))
b=int(input("enter value of b:"))
if operation == 1:
    print (a, "+", b, "=", addition(a, b))

elif operation == 2:
    print (a, "-", b, "=", subtraction(a, b)) 

elif operation == 3:
    print (a, "*", b, "=", multiplication(a, b)) 
    
elif operation == 4:
    print (a, "/", b, "=", division(a, b)) 
    
else:
    print("Invalid Input")

    
#password generator
import random
import string
allcharacters=string.alph+string.num+string.punct
length=int(input("enter the length of password:")
password = ''.join(random.choices(allcharacters, k=length))
print("Your password is:", password)
#for generaring multiple passwords
import random
import string

def generate_password(length, count):
    passwords = []
    for i in range(count):
        password = ''.join(random.choice(string.ascii_letters + string.digits + string.punctuation) for _ in range(length))
        passwords.append(password)
    return passwords

    
#create rock,paper ,scissor game using pyhton
# import random module
import random
import random
# print multiline instruction
# performstring concatenation of string
print('Winning rules of the game ROCK PAPER SCISSORS are :\n'
      + "Rock vs Paper -> Paper wins \n"
      + "Rock vs Scissors -> Rock wins \n"
      + "Paper vs Scissors -> Scissor wins \n")
 
while True:
     
    print("Enter your choice \n 1 - Rock \n 2 - Paper \n 3 - Scissors \n")
     
    # take the input from user
     
    choice=int(input("Enter your choice :"))
     
     # OR is the short-circuit operator
    # if any one of the condition is true
    # then it return True value
     
    # looping until user enter invalid input
    while choice > 3 or choice <1:
      choice=int(input('Enter a valid choice please ☺'))
         
        # initialize value of choice_name variable
# corresponding to the choice value
    if choice == 1:
        choice_name= 'Rock'
    elif choice == 2:
        choice_name= 'Paper'
    else:
        choice_name= 'Scissors'
         
        # print user choice
    print('User choice is \n',choice_name)
    print('Now its Computers Turn....')
     
    # Computer chooses randomly any number
    # among 1 , 2 and 3. Using randint method
    # of random module
    comp_choice = random.randint(1,3)
     
    # looping until comp_choice value
    # is equal to the choice value
    while comp_choice == choice:
        comp_choice = random.randint(1,3)
         
     # initialize value of comp_choice_name
    # variable corresponding to the choice value
    if comp_choice == 1:
        comp_choice_name = 'rocK'
    elif comp_choice == 2:
        comp_choice_name = 'papeR'
    else:
        comp_choice_name = 'scissoR'
    print("Computer choice is \n", comp_choice_name)
print(choice_name,'Vs',comp_choice_name)
    # we need to check of a draw
    if choice == comp_choice:
        print('Its a Draw',end="")
        result="DRAW"
    # condition for winning      
    if (choice==1 and comp_choice==2):
        print('paper wins =>',end="")
        result='papeR'
    elif (choice==2 and comp_choice==1):
        print('paper wins =>',end="")
        result='Paper'
         
       
    if (choice==1 and comp_choice==3):
        print('Rock wins =>\n',end= "")
        result='Rock'
    elif (choice==3 and comp_choice==1):
        print('Rock wins =>\n',end= "")
        result='rocK'
         
    if (choice==2 and comp_choice==3):
        print('Scissors wins =>',end="")
        result='scissoR'
    elif (choice==3 and comp_choice==2):
        print('Scissors wins =>',end="")
        result='Rock'
     # Printing either user or computer wins or draw
    if result == 'DRAW':
        print("<== Its a tie ==>")
if result == choice_name:
        print("<== User wins ==>")
    else:
        print("<== Computer wins ==>")
    print("Do you want to play again? (Y/N)")
    # if user input n or N then condition is True
    ans = input().lower()
    if ans =='n':
        break
# after coming out of the while loop
# we print thanks for playing
print("thanks for playing")


