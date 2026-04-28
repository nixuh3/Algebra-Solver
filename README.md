# Algebra-Solver

A simple C++ algebra solver for evaluating and solving equations.

## Features

- Solve **linear** and **quadratic equations (1 variable)**
- Custom variable names (alphanumeric, must not conflict with function names)
- Supports standard arithmetic:
  - Addition `+`
  - Subtraction `-`
  - Multiplication `*` (implicit multiplication allowed, eg. `3x`)
  - Division `/`
  - Powers `^`
- Built-in math functions:
  - `sin`, `cos`, `tan`
  - `asin`, `acos`, `atan`
  - `log`, `ln`
  - `sqrt`, `floor`, `ceil`, `abs`
- Built-in constants:
  - `pi`, `e`, `phi`

## Example

```
> 2x ^ 2 + 4x - 6 = 0
1
-3

> x = sin(10)
0.1736481777

```

## Requirements

- CMake ≥ 3.16
- C++20
- A compatible compiler (GCC, Clang, MSVC)

## Build Instructions

1. Clone the repository

```bash
git clone https://github.com/nixuh3/Algebra-Solver.git
cd Algebra-Solver
```

2. Configure project

```bash
cmake -S . -B build
```

3. Build

```bash
cmake --build build
```

4. Run

```bash
./build/Algebra-Solver
```

## Notes

- Enter `quit` to exit
- Equations must include exactly one variable
- Spaces are optional but recommended
- Trigonometric functions use **degrees (not radians)**
- Invalid expressions may result in errors which currently terminate the program (improvements planned)

## Contributing

Pull requests are welcome. For major changes, open an issue first.

## License

MIT License

## Todo

- Improve error messages and diagnostics
- Support systems of equations (multiple variables)
- Add higher-degree polynomial solving
- Add inequality solving
- Allow variables inside function arguments (e.g., sin(2x))
- Improve parsing and edge case handling
- Add commands such as `simplify` and `factorize`
