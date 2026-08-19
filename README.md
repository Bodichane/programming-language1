# Introduction to C++ programming

A collection of first-year lab exercises (ТКИ program), written in C++ and
documented with Doxygen (comments in Russian). Each task isolates one concept:
functions and formula evaluation, keyboard input, branching, loops and arrays.

## Organization

The repository is structured into four series of three exercises, each in its own
subfolder with its own `main.cpp`:

| Series | Topic | Exercises |
|---|---|---|
| **Task 1** | Functions and formula evaluation | multi-variable `f(x,y,z)` · weight conversion · work of an electric motor (I, U) |
| **Task 2** | Functions with several outputs | rectangle perimeter & area · piecewise function · cumulative travel time |
| **Task 3** | Branching and series | function domain of definition · sum of a recurrent sequence · pointwise evaluation |
| **Task 4** | Arrays | three operations on arrays entered at runtime |

Each exercise follows the same convention: documented prototypes at the top of
the file, `main()` for input/output, then the function definitions.

## Build and run

Each exercise is self-contained. From the repository root:

```bash
g++ -std=c++17 "Task 1/Task 1 - 1/main.cpp" -o task1-1
./task1-1
```

The programs read their parameters from standard input. The prompts and messages
shown are in Russian.

## Build status

All thirteen exercises compile without errors with `g++ -std=c++17`, verified by
compiling each one. Two fixes were needed (see the git history): an uninitialized
constant read from the keyboard in `Task 1 - 2`, and in `Task 3-2` a wrongly
retrieved count, a sum that always returned `0.0`, and a duplicated default
argument.
