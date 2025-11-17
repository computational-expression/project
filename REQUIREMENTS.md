# Project Requirements Checklist

Use this checklist to track your progress and ensure you meet all requirements.

## Code Structure Requirements

### New Concept

- [ ] Hardware project: add one new hardware component
- [ ] Software only project: add one new concept not covered in class (new data structure, reading/writing to files, graphics, API integration, etc.)

### Classes & Organization
- [ ] Have at least 2 classes (each in separate files recommended)
- [ ] Each class has a module-level docstring
- [ ] Each class has a class-level docstring
- [ ] Classes are organized logically (separation of concerns)
- [ ] Have a `main.py` file that orchestrates the application

### Functions & Methods
- [ ] Total of at least 12 functions/methods across all classes
- [ ] At least 8 functions have parameters
- [ ] At least 8 functions return values (not just `None`)
- [ ] All functions/methods have docstrings
- [ ] Docstrings include description, Args, and Returns

### Data Types & Structures
- [ ] Use at least 5 different data types (int, float, str, list, dict, tuple, bool, etc.)
- [ ] Use at least 2 lists meaningfully (not just for iteration)
- [ ] Use at least 2 dictionaries meaningfully (for data organization)
- [ ] Use lists and dicts for actual data storage/processing

### Control Flow
- [ ] At least 5 `if` statements across the codebase
- [ ] At least 3 `elif` statements
- [ ] At least 3 `else` statement
- [ ] At least 2 `for` loops
- [ ] At least 1 `while` loop

### Operators
- [ ] Use at least one arithmetic operator (+, -, *, /, //, %)
- [ ] Use at least one comparison operator (==, !=, <, >, <=, >=)
- [ ] Use at least one logical operator (and, or, not)
- [ ] Use at least one string operation (concatenation, formatting)

---

## Error Handling & Edge Cases

### Input Validation
- [ ] Validate numeric input (type checking, range checking)
- [ ] Validate string input (length, format, allowed characters)
- [ ] Handle empty input gracefully
- [ ] Provide helpful error messages to users

### Hardware Failure Handling (if applicable)
- [ ] Handle sensor read failures
- [ ] Handle connection errors gracefully
- [ ] Implement retry logic or fallback values
- [ ] Program doesn't crash on hardware errors

### Edge Case Handling
- [ ] Handle empty lists/dictionaries
- [ ] Handle boundary conditions (zero values, negative numbers)
- [ ] Handle missing or incomplete data
- [ ] Use try/except blocks appropriately
- [ ] Catch specific exceptions (not just bare `except:`)

---

## Code Quality

### Documentation
- [ ] Module-level docstring in each `.py` file
- [ ] Docstring for each class
- [ ] Docstring for each function/method
- [ ] Comments explaining complex logic
- [ ] README explaining project and how to run

### Clean Code
- [ ] Meaningful variable and function names
- [ ] Consistent naming conventions (snake_case for variables)
- [ ] No unused imports or variables
- [ ] Code is readable and well-organized
- [ ] Proper indentation and spacing

### Design Patterns
- [ ] Classes have clear responsibilities
- [ ] No unnecessary code duplication
- [ ] Good separation of concerns
- [ ] Methods are reasonably sized (not too long)

---

## Version Control

### Branching
- [ ] Created at least 2 feature branches
- [ ] Branch names are descriptive (e.g., `feature/user-auth`)
- [ ] Main/master branch remains stable
- [ ] All feature work is done in branches

### Commits
- [ ] At least 15+ commits total
- [ ] Commit messages are descriptive and clear
- [ ] Commit messages explain "why" not just "what"
- [ ] Commits represent logical units of work
- [ ] No massive commits combining many unrelated changes

### Pull Requests
- [ ] Submitted at least 2 pull requests
- [ ] Each PR has a descriptive title and description
- [ ] PR descriptions explain what changed and why
- [ ] PR descriptions mention which requirements they fulfill
- [ ] PRs include how to test the changes
- [ ] Each PR was reviewed and approved by TL

### Git Workflow Examples

**Good PR Description:**
```
## Summary
Implement user authentication system with validation

## Changes
- Added User class with password hashing
- Created login/register functionality
- Added input validation for usernames and passwords

## How to Test
1. Run: python3 src/main.py
2. Select "Register"
3. Try registering with invalid inputs
4. Should see error messages and not crash

## Requirements Met
- New coding concept: Password hashing
- Error handling: Input validation
- Classes: User, Session
- Functions: login(), register(), validate_password()
```

---

## Code Review Preparation

### What to Expect
- [ ] TL will review your code on screen
- [ ] You'll explain design decisions
- [ ] You'll answer questions about your implementation
- [ ] You may be asked to whiteboard key components
- [ ] You may need to reproduce parts of code

### Things to Know Well
- [ ] Why you designed classes the way you did
- [ ] How your error handling works
- [ ] How key algorithms function
- [ ] The flow of your main application
- [ ] Edge cases you handle

### Whiteboard Practice
- [ ] Practice explaining key functions out loud
- [ ] Be able to draw class diagrams
- [ ] Understand call flows between methods
- [ ] Know pseudocode for complex logic

---

## Presentation Preparation

### Content (5 minutes)
- [ ] **Overview (2-3 min):** Clear problem statement, key features, design decisions
- [ ] **Demo (2 min):** Live running program, 2-3 features, error handling

### Presentation Checklist
- [ ] Slides or outline prepared
- [ ] Program runs without errors
- [ ] Demo is rehearsed and smooth
- [ ] Hardware demo works (if applicable)
- [ ] Can answer questions about code
- [ ] Time limit is met (≤5 minutes)

### Assessment Rubric (see separate file)
- [ ] Clarity of explanation
- [ ] Code quality demonstrated
- [ ] Program runs correctly
- [ ] Demo is complete and smooth
- [ ] Requirements are met

---

## Final Submission Checklist

- [ ] All code is in `src/` directory
- [ ] `main.py` runs without errors
- [ ] `writing/report.md` is complete (500-800 words)
- [ ] All docstrings are present and complete
- [ ] README explains the project
- [ ] `.gitignore` is present
- [ ] Git history is clean (good commit messages)
- [ ] At least 2 PRs merged
- [ ] Code follows all requirements above
- [ ] Presentation is prepared and rehearsed

---

## Timeline Tracking

- [ ] **Nov 17-24:** Design phase complete, repo created
- [ ] **Nov 25-Dec 1:** PR #1 submitted and approved
- [ ] **Dec 2-8:** PR #2 submitted and approved
- [ ] **Dec 8:** Code reviews completed with TL
- [ ] **Dec 8:** Final presentation delivered

---

## Additional Resources

- Lab reference code (Classes, error handling, etc.)
- Python documentation: https://docs.python.org/3/
- Git guide: https://git-scm.com/book/en/v2
- Markdown guide: https://guides.github.com/features/mastering-markdown/

---

**Good luck with your project! Start early and commit often.** 🚀
