# project1
# Rock paper scissors
import random
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
game_images=[rock,paper,scissors]
user_choice=int(input("what do you choose? type 0 for rock, type 1 for paper, type 2 for scissors"))
computer_choice=random.randint(0,2)

print(game_images[computer_choice])
print(f"computer choice:{computer_choice}")
if user_choice >=3 or computer_choice<0:
    print("u entered a invalid number.you lose")

elif user_choice==0 and computer_choice==2:
    print("you wins")
    print(game_images[user_choice])
elif user_choice>computer_choice<=2:
    print("you win")
elif computer_choice==2 and user_choice==0:
    print("you lose")

elif computer_choice>user_choice<=2:
    print("you lose")
elif computer_choice== user_choice:
    print("it's a draw.")
else:
    print("you typed a invalid number. you lose")
