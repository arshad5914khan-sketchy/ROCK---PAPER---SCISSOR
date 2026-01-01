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

rock_paper_scisscors = int(input("What is your choice? 0 (Rock), 1 (Paper), 2 (Scissors): "))
random_choice = random.randint(0, 2)

# Draws
if rock_paper_scisscors == 0:
    if random_choice == 0:
        print(f"your choice {rock}")
        print(f"computer choice {rock}")
        print("computer choice:ROCK(0)")
        print("Draw")
if rock_paper_scisscors == 1:
    if random_choice == 1:
        print(f"your choice {paper}")
        print(f"computer choice {paper}")
        print("computer choice:PAPER(1)")
        print("Draw")
if rock_paper_scisscors == 2:
    if random_choice == 2:
        print(f"your choice {scissors}")
        print(f"computer choice {scissors}")
        print("computer choice:SCISSCORS(2)")
        print("Draw")

# Outcomes
if rock_paper_scisscors == 1:
    if random_choice == 0:
        print(f"your choice {paper}")
        print(f"computer choice {rock}")
        print("computer choice:ROCK(0)")
        print("You win")
        print("paper beats rock")
if rock_paper_scisscors == 2:
    if random_choice == 0:
        print(f"your choice {scissors}")
        print(f"computer choice {rock}")
        print("computer choice:ROCK(0)")
        print("You lose")
        print("rock beats scisscors")
if rock_paper_scisscors == 0:
    if random_choice == 1:
        print(f"your choice {rock}")
        print(f"computer choice {paper}")
        print("computer choice:PAPER(1)")
        print("You lose")
        print("paper beats rock")
if rock_paper_scisscors == 2:
    if random_choice == 1:
        print(f"your choice {scissors}")
        print(f"computer choice {paper}")
        print("computer choice:PAPER(1)")
        print("You win")
        print("scisscors beat paper")
if rock_paper_scisscors == 0:
    if random_choice == 2:
        print(f"your choice {rock}")
        print(f"computer choice {scissors}")
        print("computer choice:SCISSCORS(2)")
        print("You win")
        print("rock beats scisscors")
if rock_paper_scisscors == 1:
    if random_choice == 2:
        print(f"your choice {paper}")
        print(f"computer choice {scissors}")
        print("computer choice:SCISSCORS(2)")
        print("You lose")
        print("scisscors beat paper")
