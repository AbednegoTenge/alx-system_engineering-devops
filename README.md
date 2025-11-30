# 0x03. Shell, init files, variables and expansions

This repository contains various shell scripts designed to demonstrate key concepts in Bash shell scripting: aliases, variables (local/global), variable expansions, arithmetic operations, and command-line tricks. Below is a brief explanation of what each script does:

## Script Explanations

| Script Name                         | Description                                                                                           |
| -------------------------------------| ----------------------------------------------------------------------------------------------------- |
| `0-alias`                           | Creates an alias `ls` that runs `rm *` (Caution: This will delete all files in the directory!).       |
| `1-hello_you`                       | Prints “hello” followed by the value of the current user (`$USER`).                                   |
| `2-paths`<br>(not provided)          | *No file with this name in listing, likely counts directories in $PATH.*                              |
| `3-paths`                           | Counts the number of directories listed in the `PATH` environment variable.                           |
| `4-global_variables`                 | Prints global environment variables using the `env` command.                                          |
| `5-local_variables`                  | Prints all local variables and environment variables using `set`.                                     |
| `6-create_local_variable`            | Creates a local variable `BEST` and assigns it the value `"School"`.                                 |
| `7-create_global_variable`           | Creates a global variable `BEST` (exported) with the value `"School"`.                               |
| `8-true_knowledge`                   | Adds `128` to the value of `TRUEKNOWLEDGE` and prints the result.                                    |
| `9-divide_and_rule`                  | Divides the value of `POWER` by the value of `DIVIDE` and prints the result.                         |
| `10-love_exponent_breath`            | Raises `BREATH` to the power of `LOVE` and prints the result.                                        |
| `11-binary_to_decimal`               | Converts the value of `BINARY` (binary number) to decimal and prints it.                             |
| `12-combinations`                    | Prints all two-letter combinations from `aa` to `zz` except `oo`.                                    |
| `13-print_float`                     | Prints the value of `NUM` as a float with two decimal places.                                        |
| `100-decimal_to_hexadecimal`         | Converts the value of `DECIMAL` variable to its hexadecimal representation and prints it.             |
| `101-rot13`                          | Reads from stdin and applies ROT13 cipher (rotate by 13 places) to the input.                        |
| `102-odd`                            | Reads from stdin and prints only odd-numbered lines.                                                 |
| `103-water_and_stir`                 | Performs a computation based on custom encoding of `WATER` and `STIR`, outputs a string in octal then maps digits to the word “bestchol”. (Special task involving variable manipulation, tr and printf.) |

## Usage

To run any script:
```bash
./<script_name>
```
For scripts that depend on environment variables, set the variable before running:
```bash
export VARIABLE_NAME=value
./<script_name>
```

> **Warning:** The `0-alias` script redefines `ls` to a dangerous command (`rm *`). Avoid running this unless you fully understand the consequences.

## Author

[Abednego Tenge](https://github.com/AbednegoTenge)
