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
#import random module
import random
#print multiline instructions
#performing concatination of string
print('Winning rules of  game are :\n'
      +"Rock vs paper->paper wins\n"
      +"rock vs scissor->scissor wins \n"
      +"paper vs scissor ->scissor wins\n")
 while True:
      print("enter choice:\n 1.rock\n 2 paper\n 3scissor\n")
      take input from user
      choice=int(input("enter your choice")
     #or is the shortcut circuit operator
     #if any one condition is true
    #then it return true value
#looping until user end
    while choice>3 or choice<1:
      choice=int(input("enter a valid choice plzz!")
         
        #initialize the value of choicename variable
#corresponding to the choice value
if choice==1:
choicename=="rock"
elif choice==2:
 choicename=="paper"
 else:
choicename="scissors"
         
        #print users choice
    print("user choice is\n choicename")
    print("now its computers turn!")
    #computer chooses randomly any number
    #among 1,2,3 using randint method of random module
    compchoice = random.randint 1,3
     
    #looping until compchoice value is equal to the choice value
    while compchoice==choice:
        compchoice==random.randint(1,3)
         
     #initialize value of compchoice name
    #variable corresponding to the compchoice
    if compchoice==1:
       compchoicename=='rock'
    elif compchoice==2:
           compchoicename=='paper'
    else:
        compchoicename=="scissors"
        
    print("comp choice is:\n",compchoicename)
print(choicename, VS,compchoicename)
   #we need to check a draw
    if choice==compchoice:
        print("its a draw:")
        result=="draw"
    #condition for winning   
    if(choice==1 & compchoice==2):
        print("paper wins->",end)
        result="paper"
   elif(choice==2 & compchoice==1):
        print("paper wins ->",end=""
        result="paper"
         
       
    if(choice==1 and compchoice==3):
       print("rock wins:\n",end="")
        result="rock"
   elif(choice==3 and compchoice==1):
       print("rock wins:\n",end=""
       result="rock"
         
    if(choice==2 and compchoice==3):
       print("scissor wins:",end="")
       result="scissor"
   elif(choice==3 and compchoice===1):
        print("scissor wins\n",end="")
        result==rock
     #printing eitther user or computer wins or draw
    if result=="draw":
       print("its a tie")
if (result==choicename):
        print("user wins:")
   else:
   print("computer wins:")
    print("Do u want to play again:(Y/N)")
    #if user input n or N then condition is true
    ans=input().lower()
    if ans=='n':
        break
#after coming out of the while loop
#we print thanks for playing
print("thanks for playing")


