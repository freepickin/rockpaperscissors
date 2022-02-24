# rockpaperscissors

rock = '''
    _______
---'   ____)
      (_____)
      (_____)
      (____)
---.__(___)
'''

paper = '''
    _______
---'   ____)____
          ______)
          _______)
         _______)
---.__________)
'''

scissors = '''
    _______
---'   ____)____
          ______)
       __________)
      (____)
---.__(___)
'''

#Write your code below this line 👇
import random


shoot = int(input("What do you choose? Type 0 for Rock, 1 for Paper or 2 for Scissors."))

if shoot == 0:
  print('''
    _______
---'   ____)
      (_____)
      (_____)
      (____)
---.__(___)
''')

if shoot == 1:
  print('''
    _______
---'   ____)____
          ______)
          _______)
         _______)
---.__________)
''')

if shoot == 2:
  print('''
    _______
---'   ____)____
          ______)
       __________)
      (____)
---.__(___)
''')

opponent = int(random.randint(1, 3))

if opponent == 0:
  print('''
    _______
---'   ____)
      (_____)
      (_____)
      (____)
---.__(___)
''')

if opponent == 1:
  print('''
    _______
---'   ____)____
          ______)
          _______)
         _______)
---.__________)
''')

if opponent == 2:
  print('''
    _______
---'   ____)____
          ______)
       __________)
      (____)
---.__(___)
''')

if shoot == 0 and opponent == 1:
  print("Paper beats rock. You lose.")
if shoot == 0 and opponent == 2:
  print("Rock beats scissors. You win!")
if shoot == 1 and opponent == 0:
  print("Paper beats rock. You win!")
if shoot == 1 and opponent == 2:
  print("Scissors beats paper. You lose!")
if shoot == 2 and opponent == 0:
  print("Rock beats scissors. You lose!")
if shoot == 2 and opponent == 1:
  print("Scissors beats paper. You win!")
if shoot == opponent:
  print("It's a draw!")

#0 for Rock, 1 for Paper or 2 for Scissors
