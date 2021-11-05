This is an easy game; Hangman.
import random
# Write your code here
print("""H A N G M A N
The game will be available soon.""")

the_word = ['python', 'java', 'kotlin', 'javascript']
make_ur_choice = random.choice(the_word)
hidden = ("-" * int((len(make_ur_choice)) - 3))
print(make_ur_choice[0:3] + hidden)
ask = input()

if ask == make_ur_choice:
    print("You survived!")
else:
    print("You lost!")
