import random
def roll_dice():
    min_value = 1
    max_value = 6
    while True:
        print("Rolling the dice...")
        dice_number = random.randint(min_value, max_value)
        print("You rolled:", dice_number)
        roll_again = input("Do you want to roll the dice again? (yes/no): ")
        if roll_again.lower() != "yes" and roll_again.lower() != "y":
            break
    print("Thank you for playing!")
roll_dice()
