Certainly! Below is a full README file for your code:

---

# Util Library

## Introduction

The Util Library provides a collection of utility functions and classes in C++. It includes functions for generating random numbers, characters, words, keys, shuffling arrays, and swapping variables, among others. These utilities can be helpful for various tasks in C++ programming, such as generating test data, implementing algorithms, or enhancing functionality in your applications.

## Features

- **Random Number Generation**: Easily generate random numbers within a specified range.
- **Random Character Generation**: Generate random characters, including lowercase letters, uppercase letters, digits, and special characters.
- **Word and Key Generation**: Generate random words and keys based on specified character types and lengths.
- **Array Manipulation**: Fill arrays with random numbers, words, or keys, and shuffle array elements.
- **Variable Swapping**: Swap variables of different data types efficiently.
- **Text Encryption and Decryption**: Encrypt and decrypt text using a simple encryption key.

## Usage

### Include Header File

To use the Util Library in your C++ project, include the `clsUtil.h` header file:

```cpp
#include "clsUtil.h"
```

### Random Number Generation

```cpp
// Seed the random number generator
clsUtil::Srand();

// Generate a random number between From and To (inclusive)
int randomNumber = clsUtil::RandomNumber(From, To);
```

### Random Character Generation

```cpp
// Generate a random character of a specific type
char randomChar = clsUtil::GetRandomCharacter(clsUtil::enCharType::CapitalLetter);
```

### Word and Key Generation

```cpp
// Generate a random word of a specified character type and length
string randomWord = clsUtil::GenerateWord(clsUtil::enCharType::MixChars, Length);

// Generate a random key with optional character type
string randomKey = clsUtil::GenerateKey(clsUtil::enCharType::CapitalLetter);
```

### Array Manipulation

```cpp
// Fill an array with random numbers within a range
int numbers[100];
clsUtil::FillArrayWithRandomNumbers(numbers, arrayLength, From, To);

// Fill an array with random words
string words[100];
clsUtil::FillArrayWithRandomWords(words, arrayLength, CharType, WordLength);

// Fill an array with random keys
string keys[100];
clsUtil::FillArrayWithRandomKeys(keys, arrayLength, CharType);

// Shuffle an array
clsUtil::ShuffleArray(numbers, arrayLength);
clsUtil::ShuffleArray(words, arrayLength);
```

### Variable Swapping

```cpp
// Swap variables of different data types
clsUtil::Swap(var1, var2);
```

### Text Encryption and Decryption

```cpp
// Encrypt text using an encryption key
string encryptedText = clsUtil::EncryptText(text, EncryptionKey);

// Decrypt text using the same encryption key
string decryptedText = clsUtil::DecryptText(encryptedText, EncryptionKey);
```

## Contributing

Contributions to the Util Library are welcome! If you find any bugs or have suggestions for improvements, please open an issue or submit a pull request on GitHub.
