import random

def guess_game():
    secret = random.randint(1, 10)
    for chance in range(3):
        guess = int(input("Guess a number (1-10): "))
        if guess == secret:
            print("🎉 Correct! You won.")
            return
        elif guess > secret:
            print("Too High!")
        else:
            print("Too Low!")
    print("Game Over! The number was:", secret)

guess_game()
