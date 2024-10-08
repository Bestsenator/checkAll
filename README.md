
# Validator Functions Repository

This repository contains a collection of Python functions designed to validate various types of input. These functions can be used to ensure that user inputs such as passwords, emails, and other required fields meet specific criteria.

## Features

- **Password Validator**: Checks if the password meets the required structure (e.g., length, special characters, uppercase, and lowercase).
- **Email Validator**: Validates the structure of an email to ensure it follows standard email formatting rules.
- **Null Check**: Ensures that the input is not null or empty.
- **Custom Validators**: Other custom validation functions tailored for specific use cases.

## Installation

You can clone this repository using the following command:

```bash
git clone https://github.com/Bestsenator/checkAll.git
```

## Usage

Here is how you can use the provided validation functions:

### Password Validator

```python
from checkBest import checkPassword

password = "YourP@ssw0rd"
if checkPassword(password):
    print("Password is valid!")
else:
    print("Password is invalid.")
```

### Email Validator

```python
from checkBest import checkEmail

email = "example@example.com"
if checkEmail(email):
    print("Email is valid!")
else:
    print("Email is invalid.")
```

### Null Check

```python
from checkBest import checkInput

input_value = ["test", 2, "test2", null]
if checkInput(input_value):
    print("Inputs is not null!")
else:
    print("Inputs is null.")
```

### Phone/Line Check

```python
from checkBest import checkPhone

input_value = "09123456789"
if checkPhone(input_value, "phone"):
    print("Inputs is valid!")
else:
    print("Inputs is invalid.")

input_value = "01234567890"
if checkPhone(input_value, "line"):
    print("Input is valid!")
else:
    print("Input is invalid.")
```

### Type Int Check

```python
from checkBest import checkInputInt

input_value = "524155"
if checkInputInt(input_value) is False:
    print("Input is not Int!")
else:
    print("Input is Int.")
```

## Functions List

- **checkPassword(password: str) -> bool**: Returns `True` if the password is valid based on predefined criteria.
- **checkEmail(email: str) -> bool**: Returns `True` if the email is valid.
- **checkInput(input_value: list) -> bool**: Returns `True` if the all inputs is not null or empty.
- **checkPhone(input_value: str, tp: str) -> bool**: Returns `True` if the input is a phone or live valid.
- **checkInputInt(input_value: any) -> bool**: Returns `False` if the input is not Int.

## Contributing

If you would like to contribute to this project, please fork the repository and submit a pull request. We welcome any improvements or additional validators.

## Contact

For any questions or inquiries, feel free to open an issue or contact me at [senator136019@gmail.com](mailto:senator136019@gmail.com).
