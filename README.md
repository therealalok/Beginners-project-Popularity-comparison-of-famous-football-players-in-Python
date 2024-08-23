# Beginners-project-Popularity-comparison-of-famous-football-players-in-Python
This project about the popularity check in social media. Cristiano Ronaldo, Lionel Messi and Neymar Jr are the examples used here.

#Social Media Fan Following


import random
choices = ["Ronaldo", "Messi", "Neymar"]
r = random.choice(choices)  

for i in range(5):
    user = input("Enter between Ronaldo, Messi, and Neymar: ").capitalize()  
    if user not in choices:
        print("Invalid input.")
        continue
    else:
        if user == r:
            print("Both inputs are about the same person.")
        elif (user == "Ronaldo" and (r == "Messi" or r == "Neymar")) or \
             (user == "Messi" and r == "Neymar"):
            print(f"{user} is more popular on social media than {r}.")
        else:
            print(f"{user} is less popular on social media than {r}.")

