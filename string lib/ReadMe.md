# clsString class documentation

**Class: clsString**

This class represents a string object with various methods to manipulate and analyze the string content.

**Data Members:**

* `_Value`: Private string member variable that stores the actual string value.

**Member Functions:**

* **Constructors:**
    * `clsString()`: Default constructor that initializes `_Value` to an empty string.
    * `clsString(string Value)`: Constructor that initializes `_Value` with the provided string value.
* **Setters and Getters:**
    * `SetValue(string Value)`: Sets the `_Value` member variable with the provided string.
    * `GetValue()`: Returns the current value of the `_Value` member variable.
    * `Value`: Property (using `__declspec(property)`) that provides get and set access to the `_Value` member variable.
* **Static Methods:**
    * `Length(string S1)`: Static method that returns the length of the provided string `S1`.
    * `CountWords(string S1)`: Static method that counts the number of words in the provided string `S1`.
    * `UpperFirstLetterOfEachWord(string S1)`: Static method that converts the first letter of each word in the provided string `S1` to uppercase.
    * `LowerFirstLetterOfEachWord(string S1)`: Static method that converts the first letter of each word in the provided string `S1` to lowercase.
    * `UpperAllString(string S1)`: Static method that converts all letters in the provided string `S1` to uppercase.
    * `LowerAllString(string S1)`: Static method that converts all letters in the provided string `S1` to lowercase.
    * `InvertLetterCase(char char1)`: Static method that inverts the case of a single character `char1`.
    * `InvertAllLettersCase(string S1)`: Static method that inverts the case of all letters in the provided string `S1`.
    * `CountLetters(string S1, enWhatToCount WhatToCount = enWhatToCount::All)`: Static method that counts the number of letters in the provided string `S1`, optionally filtering by letter case (`enWhatToCount` enum).
    * `CountCapitalLetters(string S1)`: Static method that counts the number of capital letters in the provided string `S1`.
    * `CountSmallLetters(string S1)`: Static method that counts the number of lowercase letters in the provided string `S1`.
    * `CountSpecificLetter(string S1, char Letter, bool MatchCase = true)`: Static method that counts the occurrences of a specific letter `Letter` in the provided string `S1`, with optional case sensitivity control.
    * `IsVowel(char Ch1)`: Static method that checks if a character `Ch1` is a vowel.
    * `CountVowels(string S1)`: Static method that counts the number of vowels in the provided string `S1`.
    * `Split(string S1, string Delim)`: Static method that splits the provided string `S1` into a vector of strings based on the specified delimiter `Delim`.
    * `TrimLeft(string S1)`: Static method that removes leading whitespace characters from the provided string `S1`.
    * `TrimRight(string S1)`: Static method that removes trailing whitespace characters from the provided string `S1`.
    * `Trim(string S1)`: Static method that removes both leading and trailing whitespace characters from the provided string `S1`.
    * `JoinString(vector<string> vString, string Delim)`: Static method that joins a vector of strings `vString` into a single string with the specified delimiter `Delim`.
    * `JoinString(string arrString[], short Length, string Delim)`: Static method that joins an array of strings `arrString` of specified length `Length` into a single string with the specified delimiter `Delim`.
    * `ReverseWordsInString(string S1)`: Static method that reverses the order of words in the provided string `S1`.
    * `ReplaceWord(string S1, string StringToReplace, string sRepalceTo, bool MatchCase = true)`: Static method that replaces all occurrences of a word `StringToReplace` with another word `sRepalceTo` in the provided string `S1`, with optional case sensitivity control.
    * `RemovePunctuations(string S1)`: Static method that removes all punctuation characters from the provided string