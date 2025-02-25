import random

def get_user_choice():

    choices = ["rock", "paper", "scissors"]
    user_choice = input("Choose Rock, Paper, or Scissors: ").strip().lower()

    if user_choice not in choices:
        print("Invalid Choice! Please Choose Rock, Paper, or Scissors.")
        return get_user_choice()
    
    return  user_choice

def get_computer_choice():

    return random.choice(["rock","paper","scissors"])

def determine_winner(user, computer):

    print(f"\n You choose: {user}")
    print(f"Computer Chose: {computer}\n")

    if user == computer:
        return "Its a tie"
    
    winning_combinations = {
        "rock": "Scissors",
        "scissors": "papers",
        "paper": "rock"
    }

    if winning_combinations[user] == computer:
        return " You WIN"
    else:
        return "You LOSE"
    
def play_game():

    while True:
        user_choice = get_user_choice()
        computer_choice = get_computer_choice()
        results = determine_winner(user_choice, computer_choice)

        print(results)

        play_game = input("\nPlay AGain? (y/n): ").strip().lower()
        if play_game != 'y':
            print("Thanks for playing")
            break
if __name__ == "__main__":
    play_game()
