# username-password-validator
A simple Python project that validates username and password using string methods and conditional statements.
user = input("Enter Your Name: ")

if " " not in user and len(user) >= 5:

    password = input("Enter Password: ")

    if password == password.strip() and len(password) >= 8:
        
        if any(ch.isdigit() for ch in password):
            print(f"Account Created Name: {user}")
            print(f"Password: {password}")
        else:
            print("Password must contain a number")

    else:
        print("Invalid Password")

else:
    print("Invalid Username")
