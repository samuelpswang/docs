# MATLAB Cheat Sheat

TODO:

## MATLAB Interface (R2022a)

### Command Window

![Command Window Screenshot](./img/command-window.png)

### Editor

![Editor Window Screenshot](./img/editor.png)

## Language Basics

### Syntax

- Comments
  - Single-line: `% <comment>`
  - Multi-line: `%{ <comment> %}`

    ```matlab
    % This is a comment in MATLAB.

    %{

    This is a multi-line comment.
    It spans two lines.
    
    }%
    ```

- Breaking Lines
  - `<code> ... <code>`

    ```matlab
    x = x + ...
        123 - 456 * 789;
    ```

- Naming Convention
  - Name variables in lower snake case.

    ```matlab
    lower_snake_case
    ```

### Types

- Numbers
- Booleans
- Char, Char Arrays, Strings

### Conditionals

- If, ElseIf, Else
  - `if <condition>` ... `elseif <condition>` ... `else` ... `end`

    ```matlab
    if x = 1
      disp('x = 1');
    elseif x = 2
      disp('x = 2');
    else
      disp('x != 1 && x != 2');
    end
    ```

### Loops

- For Loop
  - `for <variable> = <start>:<end>` ... `end` (automatically asuume increment is 1)
  - `for <variable> = <start>:<increment>:<end>` ... `<end>` (increment specified)

    ```matlab
    for index = 5:-1:1
        disp(index);
    end
    ```

- While Loop
  - `while <condition>` ... `end`

    ```matlab
    while index != 5
      index = index + 1
    end
    ```

### Printing

- Display In Console
  - `disp(<something>)`

    ```matlab
    disp('display function');
    disp([1, 2, 3, 4]);
    ```

- Print As String
  - `sprintf(<print-format-string>, <variable1> ...)`
  - Takes an C-styled print format string and variables to be inserted.
  - Returns an array with formatted string and error message, use array with variables to catch result, such as: `[str, err]`.

    ```matlab
    print_string = 'x = %d';
    [string, err_msg] = sprintf(print_string, 1);
    ```

- Print To File
  - `fprintf(<print-format-string>, <variable1> ...)`
  - Display in command line, same as `disp` command.
  - Takes an C-styled print format string and variables to be inserted.

    ```matlab
    fprintf('x = %d', 1);
    ```

- C-Style Printing Statements
  - Basic Variables Used
    - Single char: `%c`
    - String: `%s`
    - Signed integer: `%d`
    - Floating point or double: `%f`

  - Floating Point Options
    - Specify number of digits before and after decimal point with `#.#`. For example: `%4.4f`.
    - Specify printing plus or minus signs with `+`. For example: `%+.2f`.

## Math

### Constants

- Pi: `pi`.
- Euler's Number / Exponential: `exp(<power>)`.

### Complex Numbers

- Declaration

  ```matlab
  % Matlab prefers "1i" to "i" or "j"
  complex_num = 1 + 1i;
  ```

- Basic Operations

  ```matlab
  % Real Part
  real(complex_num);

  % Imaginary Part
  imag(complex_num);

  % Modulus
  abs(complex_num);
  ```

- Arithmetic Operations

  ```matlab
  % Behaves as expected
  c4 = c1 * (c2 + c3);
  c6 = sqrt(c5);
  c7 = exp(2 * 1i);
  ```

### Trigonometry Functions

- Trig
  - Sine, Cosine, Tangent
- Arc
  - Arcsine, Arccosine, Arctangent

## Matrices (Arrays)

### Declaration

- Hard-code
  - `<variable> = [<element1>, <element2>, ...]`

    ```matlab
    some_array = [1, 2, 3];
    ```

- Linear Space
  - `linspace(<start>, <end>, <number-of-points>)`

    ```matlab
    some_array = linspace(0, 4, 5);
    ```

### Operations

- Accessing
  - Get element: `<variable>(<row>, <column>)`
  - Get row: `<variable>(<row>)`
  - Get column (transpose than row): `<variable>'(<column>)`

    ```matlab
    row = matrix(1);
    column = matrix'(1);
    element = matrix(1, 1);
    ```

#### Basic Operations

TODO:

## Data Visualization

### Scatter Plots

## References

- MATLAB Official Documentation ([https://uk.mathworks.com/help/matlab/index.html](https://uk.mathworks.com/help/matlab/index.html))
- Imperial College Electrical & Electronics Engineering Department MATLAB Self-Revision Course ([https://www.imperial.ac.uk/electrical-engineering](https://www.imperial.ac.uk/electrical-engineering))
