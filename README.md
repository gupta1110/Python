# Python
Programming in Python
Write python program to print first letter of your name 
a) Example: Peter
               *      *
               *             *
               *              *
               *      *
               *
               *
               *
b) Print your name by using for loop

c) check the user name is palindrome or not


ANSWER:-

def print_first_letter(name):
    first_letter = name[0].upper()
    for i in range(7):
        if i == 0:
            print("  ", "*" * 4)
        elif i == 1:
            print("  ", "*", " " * 8, "*")
        elif i == 2:
            print("  ", "*", " " * 9, "*")
        elif i == 3:
            print("  ", "*", " " * 10, "*")
        elif i == 4:
            print("  ", "*" * 2)
        elif i > 4 and i < 7:
            print("  ", "*")
        else:
            print()

def print_name_with_for_loop(name):
    for letter in name:
        print(letter.upper())

def is_palindrome(word):
    return word == word[::-1]

# a) Print the first letter with stars
print("Printing first letter of my name:")
print_first_letter("Peter")
print()

# b) Print the name using a for loop
print("Printing name using a for loop:")
print_name_with_for_loop("Peter")
print()

# c) Check if a name is a palindrome
user_name = input("Enter a name to check if it's a palindrome: ")
if is_palindrome(user_name):
    print(user_name, "is a palindrome!")
else:
    print(user_name, "is not a palindrome.")
