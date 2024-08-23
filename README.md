# OTP-Gen
# Random Password Generator

## Overview

This project provides Python scripts for generating random passwords. The scripts use different methods to create secure passwords with varying lengths and character sets, making them suitable for various applications that require password generation.

## Features

- **Generate Random Passwords**: Creates passwords with a mix of uppercase letters, lowercase letters, and digits.
- **Customizable Length**: Specify the length of the generated password.
- **Multiple Methods**: Includes different methods for generating random passwords.

## Installation

To use the password generator, you need Python installed on your system. Python 3.x is recommended.

1. Clone the repository:

    ```bash
    git clone https://github.com/your-username/random-password-generator.git
    cd random-password-generator
    ```

2. (Optional) Set up a virtual environment:

    ```bash
    python -m venv venv
    source venv/bin/activate   # On Windows, use `venv\Scripts\activate`
    ```

## Usage

### Method 1: Basic Random Password Generation

1. Open the `basic_rand_pass.py` script in a text editor or IDE.

2. Run the script using Python:

    ```bash
    python basic_rand_pass.py
    ```

3. This script will generate and print a random password of 11 characters.

### Method 2: Enhanced Random Password Generation

1. Open the `enhanced_rand_pass.py` script in a text editor or IDE.

2. Run the script using Python:

    ```bash
    python enhanced_rand_pass.py
    ```

3. This script will generate and print a random password of 10 characters.

### Method 3: Experimental Random Password Generation

1. Open the `experimental_rand_pass.py` script in a text editor or IDE.

2. Run the script using Python:

    ```bash
    python experimental_rand_pass.py
    ```

3. This script is an experimental method for generating random passwords. Note that the current implementation may not be functional and is provided for illustrative purposes.

## Example Scripts

### `basic_rand_pass.py`

```python
import string
import random

def rand_pass(size):
    gen = ''.join([random.choice(string.ascii_uppercase +
                                 string.ascii_lowercase +
                                 string.digits) for i in range(size)])
    return gen

pd = rand_pass(11)
print(pd)
