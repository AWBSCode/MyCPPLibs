# Documentation for clsString class

**Purpose:**
The `clsString` class provides various functionalities for manipulating string objects. It encapsulates common string operations such as calculating length, counting words, changing letter cases, counting specific letters, counting vowels, splitting, trimming, joining strings, reversing words, replacing words, and removing punctuations.

**Class Declaration:**
```cpp
class clsString
```

**Member Variables:**
- `_Value`: A private member variable of type `string` which holds the actual string value.

**Constructors:**
- `clsString()`: Default constructor which initializes `_Value` to an empty string.
- `clsString(string Value)`: Constructor with parameter to initialize `_Value` with a given string.

**Public Member Functions:**
1. **GetValue:**
   - Signature: `string GetValue()`
   - Description: Retrieves the current value of the string.
   - Returns: A string containing the current value.

2. **SetValue:**
   - Signature: `void SetValue(string Value)`
   - Description: Sets a new value for the string.
   - Parameters:
     - `Value`: The new value to set.

3. **Length:**
   - Signature (Static): `static short Length(string S1)`
   - Signature (Non-Static): `short Length()`
   - Description: Calculates the length of the string.
   - Parameters (Static): `S1` - The string to calculate the length for (optional for non-static version).
   - Returns: The length of the string.

4. **CountWords:**
   - Signature (Static): `static short CountWords(string S1)`
   - Signature (Non-Static): `short CountWords()`
   - Description: Counts the number of words in the string.
   - Parameters (Static): `S1` - The string to count words for (optional for non-static version).
   - Returns: The count of words.

5. **UpperFirstLetterOfEachWord:**
   - Signature (Static): `static string UpperFirstLetterOfEachWord(string S1)`
   - Description: Converts the first letter of each word to uppercase.
   - Parameters: `S1` - The string to modify.
   - Returns: The modified string.

6. **LowerFirstLetterOfEachWord:**
   - Signature (Static): `static string LowerFirstLetterOfEachWord(string S1)`
   - Description: Converts the first letter of each word to lowercase.
   - Parameters: `S1` - The string to modify.
   - Returns: The modified string.

7. **UpperAllString:**
   - Signature (Static): `static string UpperAllString(string S1)`
   - Description: Converts the entire string to uppercase.
   - Parameters: `S1` - The string to modify.
   - Returns: The modified string.

8. **LowerAllString:**
   - Signature (Static): `static string LowerAllString(string S1)`
   - Description: Converts the entire string to lowercase.
   - Parameters: `S1` - The string to modify.
   - Returns: The modified string.

9. **InvertAllLettersCase:**
   - Signature (Static): `static string InvertAllLettersCase(string S1)`
   - Description: Inverts the case of all letters in the string.
   - Parameters: `S1` - The string to modify.
   - Returns: The modified string.

10. **CountLetters:**
    - Signature (Static): `static short CountLetters(string S1, enWhatToCount WhatToCount = enWhatToCount::All)`
    - Description: Counts the number of letters in the string based on specified criteria.
    - Parameters:
      - `S1`: The string to count letters for.
      - `WhatToCount`: Enum specifying whether to count small letters, capital letters, or all letters (default: All).
    - Returns: The count of letters.

11. **CountCapitalLetters:**
    - Signature (Static): `static short CountCapitalLetters(string S1)`
    - Description: Counts the number of capital letters in the string.
    - Parameters: `S1` - The string to count capital letters for.
    - Returns: The count of capital letters.

12. **CountSmallLetters:**
    - Signature (Static): `static short CountSmallLetters(string S1)`
    - Description: Counts the number of small letters in the string.
    - Parameters: `S1` - The string to count small letters for.
    - Returns: The count of small letters.

13. **CountSpecificLetter:**
    - Signature (Static): `static short CountSpecificLetter(string S1, char Letter, bool MatchCase = true)`
    - Description: Counts the occurrences of a specific letter in the string.
    - Parameters:
      - `S1`: The string to search for the letter.
      - `Letter`: The letter to count.
      - `MatchCase`: Flag to indicate whether to match case (default: true).
    - Returns: The count of occurrences.

14. **CountVowels:**
    - Signature (Static): `static short CountVowels(string S1)`
    - Signature (Non-Static): `short CountVowels()`
    - Description: Counts the number of vowels in the string.
    - Parameters (Static): `S1` - The string to count vowels for (optional for non-static version).
    - Returns: The count of vowels.

15. **Split:**
    - Signature (Static): `static vector<string> Split(string S1, string Delim)`
    - Signature (Non-Static): `vector<string> Split(string Delim)`
    - Description: Splits the string into substrings based on a delimiter.
    - Parameters (Static): `S1` - The string to split.
    - Parameters (Non-Static): `Delim` - The delimiter to split the string by.
    - Returns: A vector of substrings.

16. **TrimLeft:**
    - Signature (Static): `static string TrimLeft(string S1)`
    - Description: Trims leading whitespace characters from the string.
    - Parameters: `S1` - The string to trim.
    - Returns: The trimmed string.

17. **TrimRight:**
    - Signature (Static): `static string TrimRight(string S1)`
    - Description: Trims trailing whitespace characters from the string.
    - Parameters: `S1` - The string to trim.
    - Returns: The trimmed string.

18. **Trim:**
    - Signature (Static): `static string Trim(string S1)`
    - Description: Trims leading and trailing whitespace characters from the string.
    - Parameters: `S1` - The string to trim.
    - Returns: The trimmed string.

19. **JoinString:**
    - Signature (Static): `static string JoinString(vector<string> vString, string Delim)`
    - Signature (Static): `static string JoinString(string arrString[], short Length, string Delim)`
    - Description: Joins an array or vector of strings into a single string with a delimiter.
    - Parameters:
      - `vString` or `arrString`: Array or vector of strings to join.
      - `Length`: Length of the array (for the array version).
      - `Delim`: Delimiter to separate each string.


    - Returns: The concatenated string.

20. **ReverseWordsInString:**
    - Signature (Static): `static string ReverseWordsInString(string S1)`
    - Description: Reverses the order of words in the string.
    - Parameters: `S1` - The string to reverse.
    - Returns: The string with reversed word order.

21. **ReplaceWord:**
    - Signature (Static): `static string ReplaceWord(string S1, string StringToReplace, string sRepalceTo, bool MatchCase = true)`
    - Description: Replaces occurrences of a word in the string with another word.
    - Parameters:
      - `S1`: The string to perform replacement on.
      - `StringToReplace`: The word to replace.
      - `sRepalceTo`: The word to replace with.
      - `MatchCase`: Flag to indicate whether to match case (default: true).
    - Returns: The modified string.

22. **RemovePunctuations:**
    - Signature (Static): `static string RemovePunctuations(string S1)`
    - Description: Removes punctuations from the string.
    - Parameters: `S1` - The string to remove punctuations from.
    - Returns: The string without punctuations.

**Conclusion:**
The `clsString` class provides a comprehensive set of string manipulation functionalities, enabling developers to perform various operations on string objects with ease and efficiency. It encapsulates common string operations in a reusable and organized manner, promoting code readability and maintainability.