import random

i = 0
password = ""

specialchar = ["!", "@", "#", "$", "%", "^", "&", "*", "-", "_", "+", ":"]
numbers = [1, 2, 3, 4, 5, 6, 7, 8, 9]
lowerletters = ["a", "b", "c", "d", "e", "f", "g", "h", "i", "j", "k", "l", "m",
                "n", "o", "p", "q", "r", "s", "t", "u", "v", "w", "x", "y", "z"]
upperletters = [letter.upper() for letter in lowerletters]

while i < 30:
    specchoice = random.choice(specialchar)
    numchoice = random.choice(numbers)
    lowchoice = random.choice(lowerletters)
    upchoice = random.choice(upperletters)
    password += specchoice + str(numchoice) + lowchoice + upchoice
    i += 1

finalpassword = password + "///////+YL77PASSWORDGENERATOR==@@$$///////"
print(f"Your password is: {finalpassword}!")
