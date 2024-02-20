# clsInputValidate

`clsInputValidate` is a C++ class designed to provide input validation functionalities for various data types and date ranges. It offers methods to validate numbers and dates and to read input from the user within specified ranges.

## Table of Contents

- [Usage](#usage)
- [Methods](#methods)
- [Examples](#examples)
- [Contributing](#contributing)
- [License](#license)

## Usage

To use `clsInputValidate` in your C++ project, include the header file `clsInputValidate.h` along with any necessary dependencies. Then, you can access the provided validation and input reading methods.

```cpp
#include "clsInputValidate.h"

// Example usage
int main() {
    // Validate a number within a range
    int num = clsInputValidate::ReadIntNumberBetween(1, 10, "Enter a number between 1 and 10: ");

    // Validate a double within a range
    double dbl = clsInputValidate::ReadDblNumberBetween(0.0, 100.0, "Enter a number between 0 and 100: ");

    // Validate a date within a range
    clsDate date = clsInputValidate::ReadDate();
    if (!clsInputValidate::IsValideDate(date)) {
        cout << "Invalid date entered. Please try again." << endl;
    }

    return 0;
}
```

## Methods

- `IsNumberBetween`: Checks if a number is within a specified range for various numeric types.
- `IsDateBetween`: Checks if a date is within a specified date range.
- `ReadIntNumber`: Reads an integer number from the console.
- `ReadIntNumberBetween`: Reads an integer number within a specified range from the console.
- `ReadDblNumber`: Reads a double number from the console.
- `ReadDblNumberBetween`: Reads a double number within a specified range from the console.
- `IsValideDate`: Checks if a date is valid.

## Examples

### Validate a Number

```cpp
int num = clsInputValidate::ReadIntNumberBetween(1, 10, "Enter a number between 1 and 10: ");
```

### Validate a Double

```cpp
double dbl = clsInputValidate::ReadDblNumberBetween(0.0, 100.0, "Enter a number between 0 and 100: ");
```

### Validate a Date

```cpp
clsDate date = clsInputValidate::ReadDate();
if (!clsInputValidate::IsValideDate(date)) {
    cout << "Invalid date entered. Please try again." << endl;
}
```

## Contributing

Contributions to improve and extend the functionality of `clsInputValidate` are welcome. Feel free to open issues for feature requests, bug reports, or general feedback.

## License

This project is licensed under the [MIT License](LICENSE).