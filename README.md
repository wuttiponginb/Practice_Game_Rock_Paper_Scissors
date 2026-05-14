print("---Game Rock, Paper, Scissors---")
import random

choice_game = ("Rock", "Paper", "Scissors")
bot = random.choice(choice_game)
while True:
    user_choice = input("Enter your choice (Rock, Paper ,Scissors): ")
    if user_choice == "Rock" or user_choice == "Paper" or user_choice == "Scissors":
        if user_choice == bot:
            print("You Draw!")
        elif user_choice == "Rock" and bot == "Scissors" or user_choice == "Paper" and bot == "Rock" or user_choice == "Scissors" and bot == "Paper":
            print("You Win!")
        elif user_choice == "Rock" and bot == "Paper" or user_choice == "Paper" and bot == "Scissors" or user_choice == "Scissors" and bot == "Rock":
            print("You Lose!")
    else:
        print("---Press enter choice Rock, Paper ,Scissors---")
