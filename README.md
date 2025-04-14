'''
This is simple project on snake, wate , gun game.
The game is played between two players, if one is snake then other is either water or gun.

'''
import random
Your_choice = input("Enter your choice (snake/water/gun): ").lower()
computer_choice = random.choice(["snake", "water", "gun"])

print(f"Computer choice: {computer_choice}")
if(Your_choice == computer_choice):
    print("It's a tie!")

elif(Your_choice == "snake"):
    if (computer_choice == "water"):
        print("You win! Snake drinks water.")
            
elif (Your_choice == "water"):
    if (computer_choice == "gun"):
        print("You win! Water drown gun.")
            
elif (Your_choice == "gun"):
    if (computer_choice == "snake"):
        print("You win! Gun shoots snake.")
            
elif (Your_choice == "snake"):
    if (computer_choice == "gun"):
        print("You lose! Gun shoots snake.")
            
elif (Your_choice == "water"):
    if (computer_choice == "snake"):
        print("You lose! Snake drinks water.")
            
elif (Your_choice == "gun"):
    if (computer_choice == "water"):
        print("You lose! Water drown gun.")
            
else:
    print("Invalid choice! Please choose snake, water, or gun.") 
             
    
