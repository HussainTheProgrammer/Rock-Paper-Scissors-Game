# Rock-Paper-Scissors-Game

import random
print("Welcome to Rock Paper Scissors Game")
print("R for Rock, P for Paper, S for Scissor")
print("Total Rounds : 10")
Elements = ("Rock", "Paper", "Scissors")
comp_win = 0
win = 0
tries = 0
tie = 0
while (tries<=10):
    a = input("Your Choice : ")
    comp = random.choice(Elements)
    if a == "R" and comp == "Paper":
        comp_win = comp_win + 1
        print("You Lost")
        f = f"Your win : {win}, Computer Win : {comp_win}"
        print(f)
        tries = tries + 1

    elif a == "R" and comp == "Scissors":
        win = win + 1
        print("You Won")
        f = f"Your win : {win}, Computer Win : {comp_win}"
        print(f)
        tries = tries + 1
        continue

    elif a == "R" and comp == "Rock":
        tie = tie + 1
        print("Tie")
        f = f"Your win : {win}, Computer Win : {comp_win}"
        print(f)
        tries = tries + 1
        continue

    elif a == "P" and comp == "Paper":
        tie = tie + 1
        print("Tie")
        f = f"Your win : {win}, Computer Win : {comp_win}"
        print(f)
        tries = tries + 1
        continue

    elif a == "P" and comp == "Scissors":
        comp_win = comp_win + 1
        print("You Lost")
        f = f"Your win : {win}, Computer Win : {comp_win}"
        print(f)
        tries = tries + 1
        continue

    elif a == "P" and comp == "Rock":
        print("You Won")
        win = win + 1
        f = f"Your win : {win}, Computer Win : {comp_win}"
        print(f)
        tries = tries + 1
        continue

    elif a == "S" and comp == "Scissors":
        tie = tie + 1
        print("Tie")
        f = f"Your win : {win}, Computer Win : {comp_win}"
        print(f)
        tries = tries + 1
        continue

    elif a == "S" and comp == "Rock":
        comp_win = comp_win + 1
        print("You Lost")
        f = f"Your win : {win}, Computer Win : {comp_win}"
        print(f)
        tries = tries + 1
        continue

    elif a == "S" and comp == "Paper":
        print("You Won")
        win = win + 1
        f = f"Your win : {win}, Computer Win : {comp_win}"
        print(f)
        tries = tries + 1
        continue
    else :
        print("Please Enter a valid element")
        break
final = f"Your Rounds : {win}, Computer Rounds : {comp_win}, Ties : {tie}"
print(final)
