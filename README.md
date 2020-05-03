# python-codes
import random

i = 0
j = 0
# lst = ["snake", "water", "gun"]
while int(i+j) < 11:
    lst = ["snake", "water", "gun"]
    user_input = str(input("enter s for snake,w for water or g for gun to start the game\n"))
    choice = random.choice(lst)
    a = str(choice)

    if a == user_input:
        print("tie")
    elif user_input == "s" and a == "water":
       p=f"pytho n made {a}"
        print=(p)
        print("you win")
        i = i+1

    elif user_input == "s" and a == "gun":
        p= f"python made {a}"
        print=(p)
        print("python wins")
        j = j + 1
    elif user_input=="w" and a == "snake":
        p=f"pytho n made {a}"
        print=(p)
        j = j+1
        print("python wins")
    elif user_input == "w" and a == "gun":
        p=f"pytho n made {a}"
        print=(p)

        print("you wins")
        i = i+1

    elif user_input == "g" and a == "snake":
        p=f"pytho n made {a}"
        print=(p)
        print("you wins")
        i = i+1

    elif user_input == "g" and a == "water":
        print(f"python made {a}")

        print("python wins")
        j = j+1

    else:
        print("please enter the given words only its case sensitive")
print("user score= ", i)
print("python score= ", j)

