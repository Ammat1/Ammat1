import random

def get_player_number(player_name):
    number = random.randint(1, 6)
    print(f"{player_name} rolled a {number}")
    return number

def game():
    player1_name = input("Enter player 1 name: ")
    player2_name = input("Enter player 2 name: ")

    player1_number = get_player_number(player1_name)
    player2_number = get_player_number(player2_name)

    if player1_number > player2_number:
        print(f"{player1_name} wins!")
    elif player1_number < player2_number:
        print(f"{player2_name} wins!")
    else:
        print("It's a tie!")

game()
