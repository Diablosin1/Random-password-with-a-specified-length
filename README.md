# Random-password-with-a-specified-length
# Here's a simple Python code that generates a random password with a specified length.

    import random
    import string

    def generate_password(length):
        characters = string.ascii_letters + string.digits + string.punctuation
        password = ''.join(random.choice(characters) for _ in range(length))
        return password

    # Prompt the user for the password length
    password_length = int(input("Enter the desired password length: "))

    # Generate and print the password
    password = generate_password(password_length)
    print("Generated Password:", password)
