# 📂 Project Structure
password_generators/
│
├── pin_generator.py
├── random_password_generator.py
├── memorable_password_generator.py
└── README.md

# 🚀 Features
## ✅ PinGenerator

Generates a numeric PIN of fixed length.

Example: 48293

## ✅ RandomPasswordGenerator

Generates a random password with customizable options:

Length (default: 8)

Include numbers

Include symbols

Example: aT9$Kd2P

## ✅ MemorablePasswordGenerator

  Generates a password from multiple words.

Options:

Number of words (default: 4)

Separator (default: _)

Random capitalization

Custom vocabulary (default: NLTK words corpus)

Example: apple_Bridge_house_Tree
***
# 🛠 Installation

1. Clone this repository:
git clone https://github.com/https://github.com/hajarrajabi/password-generators.git
cd password-generators
2. Install dependencies:

     pip install nltk


3. (Optional) Download NLTK word corpus if you plan to use the memorable generator:

    import nltk
nltk.download("words")
***

# 📌 Usage
from pin_generator import PinGenerator
from random_password_generator import RandomPasswordGenerator
from memorable_password_generator import MemorablePasswordGenerator

## PIN Generator
pin_gen = PinGenerator(length=6)
print(pin_gen.generate())  # e.g., "593821"

## Random Password Generator
rand_gen = RandomPasswordGenerator(length=12, include_number=True, include_symbol=True)
print(rand_gen.generate())  # e.g., "a8$TrLz9!XpQ"

## Memorable Password Generator
mem_gen = MemorablePasswordGenerator(number_of_words=4, separator="-", capitalize=True)
print(mem_gen.generate())  # e.g., "Dog-tree-River-CAT"

***
## 📜 License

This project is licensed under the MIT License.

