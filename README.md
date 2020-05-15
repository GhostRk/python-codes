# python-codes
import random
k=0
i = 0
j = 0
# lst = ["snake", "water", "gun"]
while int(i+j+k) < 10:
    lst = ["snake", "water", "gun"]
    user_input = str(input("enter s for snake,w for water or g for gun to start the game\n"))
    choice = random.choice(lst)
    a = str(choice)

    if user_input == "s" and a == "water":
        print(f"pytho n made {a}")
        print("you win")
        i = i+1

    elif user_input == "s" and a == "gun":

        print(f"pytho n made {a}")
        print("python wins")
        j = j + 1
    elif user_input=="w" and a == "snake":

        print(f"pytho n made {a}")
        j = j+1
        print("python wins")
    elif user_input == "w" and a == "gun":

        print(f"pytho n made {a}")

        print("you wins")
        i = i+1

    elif user_input == "g" and a == "snake":

        print(f"pytho n made {a}")
        print("you wins")
        i = i+1

    elif user_input == "g" and a == "water":
        print(f"python made {a}")

        print("python wins")
        j = j+1

    else:	
    			print("Tie")
    			k+=1
print("user score= ", i)
print("python score= ", j)
if i>j:
	print("user wins")
elif i==j:
	print("tie game")
else:print(")
	

