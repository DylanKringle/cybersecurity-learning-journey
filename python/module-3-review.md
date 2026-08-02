# Python Module 3 Review

## Status

Completed and reviewed.

## Score Summary

| Topic | Score |
| --- | ---: |
| Loops | 10/10 |
| Counters | 10/10 |
| Boolean switches | 10/10 |
| Building strings | 10/10 |
| String methods | 9.5/10 |
| Debugging | 9/10 |
| Overall Module 3 | 9.8/10 |

The autograder displayed `110/100`; the meaningful evidence is that all listed tests passed.

## Programs Practiced

- `analyze_text()`
- `is_strong_pw(password)`
- `numberify(word)`

## Concepts Practiced

- Defining and calling functions
- Parameters and arguments
- Function scope
- `return` versus `print`
- Using `main()` to coordinate a program
- Loops over strings
- Counters
- Boolean switches
- Building new strings
- String methods such as `isupper()`, `islower()`, `isdigit()`, and `upper()`
- Membership checks such as `if char in "aeiou"`
- `len()`
- Independent `if` checks versus `if` / `elif` / `else`
- Debugging syntax, indentation, variable, type, and logic errors

## What I Learned

This module helped me understand how to inspect and transform strings one character at a time. I practiced deciding whether a problem requires counting, remembering whether something happened, or building a new string.

One important distinction was learning when a function should `return` a value instead of only using `print()`. Returning a value makes the function reusable and testable, which matters for future automation and security scripts.

## Common Mistakes I Practiced Fixing

- Forgetting method parentheses, such as writing `char.isdigit` instead of `char.isdigit()`
- Mixing up method names, such as guessing `isuppercase()` instead of `isupper()`
- Starting a string builder with `0` instead of `""`
- Using inconsistent variable names
- Indentation mistakes
- Confusing parameter names with variables outside the function

## Cybersecurity Connection

These patterns connect directly to future cybersecurity work:

- Counting failed login attempts in logs
- Checking whether passwords meet simple rules
- Transforming or sanitizing text
- Validating user input
- Building small automation scripts

## Verification

Evidence for completion:

- Rewrote programs
- Debugged errors after running code
- Solved modified practice problems
- Explained why the code worked
- Passed the listed autograder tests
