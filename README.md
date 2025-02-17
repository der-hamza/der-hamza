- 👋 Hi, I’m @der-hamza
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
der-hamza/der-hamza is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
print("Welcome to Python Pizza Deliveries!")
bill = 0
size = input("What size pizza do you want? S, M or L: ")
pepperoni = input("Do you want pepperoni on your pizza? Y or N: ")
extra_cheese = input("Do you want extra cheese? Y or N: ")

if size == "S":
    bill += 15
elif size == "M":
    bill += 20
elif size == "L":
    bill += 25
else :
    print("You typed the wrong inputs.")
    
if pepperoni == "Y":
    if size == "S":
        bill += 2
    else :
        bill += 3
if extra_cheese == "Y":
    bill += 1   

print(f"Your final bill is:$ {bill}.") 

#Treasure Islands
print('''
*******************************************************************************
          |                   |                  |                     |
 _________|________________.=""_;=.______________|_____________________|_______
|                   |  ,-"_,=""     `"=.|                  |
|___________________|__"=._o`"-._        `"=.______________|___________________
          |                `"=._o`"=._      _`"=._                     |
 _________|_____________________:=._o "=._."_.-="'"=.__________________|_______
|                   |    __.--" , ; `"=._o." ,-"""-._ ".   |
|___________________|_._"  ,. .` ` `` ,  `"-._"-._   ". '__|___________________
          |           |o`"=._` , "` `; .". ,  "-._"-._; ;              |
 _________|___________| ;`-.o`"=._; ." ` '`."\` . "-._ /_______________|_______
|                   | |o;    `"-.o`"=._``  '` " ,__.--o;   |
|___________________|_| ;     (#) `-.o `"=.`_.--"_o.-; ;___|___________________
____/______/______/___|o;._    "      `".o|o_.--"    ;o;____/______/______/____
/______/______/______/_"=._o--._        ; | ;        ; ;/______/______/______/_
____/______/______/______/__"=._o--._   ;o|o;     _._;o;____/______/______/____
/______/______/______/______/____"=._o._; | ;_.--"o.--"_/______/______/______/_
____/______/______/______/______/_____"=.o|o_.--""___/______/______/______/____
/______/______/______/______/______/______/______/______/______/______/[TomekK]
*******************************************************************************
''')
print("Welcome to the treasure Island.")
print("Your mission is to find the treasure.")
step_1 = input("You are at the cross road. Where do you want to go? \n Please type left or right :")

#step_3 = input("Which door you want to open? \n Please type red, yellow or blue")

if step_1 == "left":
    step_2 = input("What you want to do now? \n Please type swim or wait :")
    if step_2 == "wait":
        step_3 = input("Which door you want to open? \n Please type red, yellow or blue :")
        if step_3 =="red":
            print("Burned by fire. Game Over")
        elif step_3 =="yellow":
            print("You win !")
        elif step_3 =="blue":
            print("Eaten by beasts. Game Over.")
        else :
            print("Game Over")
    else :
        print("Attacked by  trout. Game Over.")
else :
    print("You fall into a hole. Game Over.")   
