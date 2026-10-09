```python
import secrets
import string

# Define the character set for password generation
alphabet = string.ascii_letters + string.digits + string.punctuation


# Function to count the occurrences of each character type in a password
def count_occurrences(password, character_set):
    return len(set(filter(lambda c: c in character_set, password)))


def assess_password_strength(password):
    strengths = []  # List of strengths of the password
    weaknesses = []  # List of weaknesses of the password

    # debug purposes print(password)
    # Count the occurrences of each character type in the password
    lowercase_count = count_occurrences(password, alphabet.lower())
    uppercase_count = count_occurrences(password, alphabet.upper())
    digit_count = count_occurrences(password, string.digits)
    special_character_count = count_occurrences(password, string.punctuation)
    # debug purposes print(lowercase_count, uppercase_count, digit_count, special_character_count)

    # Identify strengths based on character type presence
    if lowercase_count > 0:
        strengths.append("Lowercase letters")
    if uppercase_count > 0:
        strengths.append("Uppercase letters")
    if digit_count > 0:
        strengths.append("Digits")
    if special_character_count > 0:
        strengths.append("Special characters")
    if len(password) >= 10:
        strengths.append("Length")
    # debug purposes print(strengths, weaknesses)

    # Identify weaknesses based on character type balance
    if (
        lowercase_count == 0
        or uppercase_count == 0
        or digit_count == 0
        or special_character_count == 0
    ):
        weaknesses.append("Missing at least one character type")
    else:
        if (
            len(password)
            / (
                lowercase_count
                + uppercase_count
                + digit_count
                + special_character_count
            )
            >= 2
        ):
            weaknesses.append("Balance between character types could be improved")
        else:
            strengths.append("Good balance between character types")

    # Assess overall password strength
    if not strengths or weaknesses:
        strength = "Weak"
    else:
        strength = "Strong"

    # debug purposes print("right before return", strengths, weaknesses)
    # Return a dictionary with the strength, weaknesses, and strengths of the password
    return strength, strengths, weaknesses


# Welcome message and input prompt for password length
print("Welcome to my password generator!")
length = 0
try:
    while True:
        try:
            # get user input for deciding how long the password is.
            length = int(input("Enter the length of the password (at least 10): "))

            if length < 10:
                raise ValueError("Password length must be at least 10.")
            break
        except ValueError as e:
            print(f"Error: {e}")

    # Initialize variables for password generation and strength assessment
    max_attempts = 10  # Maximum number of attempts to generate a strong password
    attempts = 0  # Counter for number of generation attempts
    password = ""  # Empty string for generated password

    # Loop until a strong password is generated or maximum attempts reached
    while attempts < max_attempts:
        password = "".join(secrets.choice(alphabet) for _ in range(length))
        # debug purposes print("generated password from while loop:", password)

        # Assess password strength and display assessment results
        strength, strengths, weaknesses = assess_password_strength(password)
        # debug purposes print("after assessing password strength", strengths, weaknesses)

        # If no weaknesses detected, mark as strong password
        if not weaknesses:
            weaknesses = ["No weaknesses!"]
            # debug purposes print("right before generated password message", strengths, weaknesses)

        print(
            f"Generated Password: {password}\nStrength: {strength}\nweaknesses: {weaknesses}\nstrengths: {strengths}"
        )

        # Stop generating passwords if a strong password is found
        if strengths and weaknesses == ["No weaknesses!"]:
            break

        # Update attempts counter
        attempts += 1

    if attempts == max_attempts:
        print(
            f"Unable to generate a strong password meeting the criteria after {max_attempts} attempts."
        )
except ValueError as e:
    print(e)
```

this took forever
