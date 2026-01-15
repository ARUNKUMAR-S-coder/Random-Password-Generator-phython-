# Random-Password-Generator-phython-
Random Password Generator – A simple Python program to generate secure, random passwords. Users can choose the number and length of passwords. Includes uppercase, lowercase, and special characters for strong, unpredictable passwords. Perfect for quick, safe password creation.
# code:- 
import random

print("Welcome to Random Password Generator")

randomchar = "ABCDEFGHIKaabcdefhijk@#€¥$"

num_passwords = int(input("Enter number of passwords required: "))
password_length = int(input("Enter length of each password: "))

for _ in range(num_passwords):
    pwd = ""
    for _ in range(password_length):
        pwd += random.choice(randomchar)
    print(pwd)
