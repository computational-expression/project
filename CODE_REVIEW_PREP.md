# Code Review Preparation Guide

## What to Expect During Code Review

**Format:**
1. TL/Instructor reviews your code in your pull request (PR)
2. **Randomly selects 3 computational concepts** from the topics we covered in class (see list below)
3. **Asks 3 questions** about how you used each concept - one question per concept
4. For each concept, the question will be one of these three types:
   - **Question Type 1:** Execution tracing - walk through your code step-by-step with specific inputs
   - **Question Type 2:** Edge cases - explain what happens with unusual or boundary inputs
   - **Question Type 3:** Code modification - make a small change to your code and trace through it
5. You use a whiteboard to **reproduce portions of your code** and explain:
   - What happens step-by-step
   - What values are stored in variables/data structures
   - How data flows through your code
6. TL/instructor approves your PR or requests changes.

**Remember:** Code reviews are not about being perfect. They are about demonstrating that you understand the code you wrote. We want to see that you can trace through your own code and explain what is happening!

---

## The Three Question Types

For each of the 3 randomly selected concepts, we will ask one question. Questions will follow one of these three patterns:

**Question Type 1: Execution Tracing**
- Walk through your code step-by-step with specific inputs
- Show how variables change, what loops/conditionals do, what functions return
- Demonstrate understanding of your actual code logic

**Question Type 2: Edge Cases & Variations**
- Explain what happens with boundary cases (empty inputs, extreme values, etc.)
- Show how your error handling works (if applicable)
- Demonstrate understanding beyond the "happy path"

**Question Type 3: Code Modification**
- Make a small modification to your code and trace through the result
- Explain what changed and why the modification has the expected effect
- Demonstrate understanding of how pieces fit together

---

## Before Your Code Review

### Prepare Your Code
- [ ] Code is clean and well-formatted
- [ ] All docstrings are complete and accurate
- [ ] Code runs without errors
- [ ] You have tested all major features
- [ ] No unused imports or variables

### Know Your Code
- [ ] Understand every line you wrote
- [ ] Be able to explain why you made design choices
- [ ] Know the flow of your main functions and loops
- [ ] Be ready to trace through code with sample inputs
- [ ] Understand what data is stored at each step
- [ ] Know your edge cases (empty lists, invalid input, etc.)

### Practice All Three Question Types
**Question Type 1: Execution Tracing**
- [ ] Trace through each loop step-by-step with specific inputs
- [ ] Show how variables change at each iteration
- [ ] Practice with different input sizes (small, large, etc.)

**Question Type 2: Edge Cases & Variations**
- [ ] Trace through your code with empty inputs
- [ ] Trace with invalid or unexpected inputs
- [ ] Show how your error handling works
- [ ] Practice explaining what happens in edge cases

**Question Type 3: Code Modification**
- [ ] Practice modifying your code on the white board
- [ ] Trace through the modified version
- [ ] Be able to explain what changed and why
- [ ] Think about alternative implementations

---

## Concepts We'll Ask About

We will **randomly select 3 concepts** from this list and ask **one question per concept** about how you used it in your code.

**Study these concepts from our slides (Weeks 2-12):**

### Python Fundamentals (Week 2)
- **Variables & Naming** - Variable assignment, naming conventions, dynamic typing, scope
- **Program Structure** - Statements, indentation, code blocks, execution flow

### Data Types & Operations (Week 3)
- **Data Types** - int, float, str, bool, list, dict; type checking with `type()`
- **Operators** - Arithmetic (+, -, *, /, //, %), comparison (==, !=, <, >, <=, >=), logical (and, or, not), string concatenation/formatting

### Control Flow - Conditionals (Week 3)
- **If/Elif/Else** - Condition evaluation, boolean logic, nested conditionals

### Control Flow - Loops (Week 4)
- **For Loops** - Iteration over sequences, range(), loop variable usage, nested loops
- **While Loops** - Loop structure, exit conditions, infinite loop risks, loop counters

### Lists (Week 6)
- **List Operations** - Indexing, slicing, append, remove, insert, length, iteration
- **List Usage** - When to use lists, list methods, searching/filtering

### Dictionaries (Week 10)
- **Dictionary Structure** - Key-value pairs, accessing values, keys(), values(), items()
- **Dictionary Usage** - When to use dicts vs lists, nested structures, iteration patterns

### Functions (Week 9)
- **Function Definition** - Parameters, return values, docstrings, scope
- **Function Design** - Single responsibility, parameter choices, return type decisions

### Object-Oriented Programming (Week 11)
- **Classes & Objects** - Class definition, `__init__`, attributes, methods, self
- **Class Design** - When to create classes, class responsibilities, interaction between classes

### Error Handling
- **Try/Except Blocks** - Exception types, catching specific exceptions, finally blocks
- **Input Validation** - Type checking, range checking, error messages

### Version Control (Week 11)
- **Git Basics** - Branches, commits, pull requests, merge conflicts
- **Workflow** - Feature branches, commit messages, code review process

### Debugging (Week 5)
- **Debugging Strategies** - Print statements, reading error messages, tracing code
- **Common Errors** - Off-by-one errors, None values, type mismatches

---

## How to Prepare for Each Question Type

### For Execution Tracing Questions
You will be asked to walk through a section of your code with specific inputs and show what happens:
- Trace through step-by-step on the whiteboard
- Show the value of each variable at key points
- Show what happens in each loop iteration
- Arrive at the final result

Be ready to trace through any part of your code, not just the simple parts.

### For Edge Case Questions
You will be asked what happens when your code encounters unusual situations:
- Think about empty inputs (empty lists, empty strings, etc.)
- Think about extreme values (very large or very small numbers, etc.)
- Think about invalid inputs (what if the user enters something unexpected?)
- Be ready to show how your code handles these situations

### For Code Modification Questions
You will be asked to make a small change to your code and trace through it:
- Make a modification on the whiteboard
- Trace through the modified code with sample input
- Explain what changed and what effect it has
- Show that you understand how the code works, not just what it does

---

## Whiteboarding Tips

When you are asked to show your work:

1. **Show the code** on the whiteboard (or point to it on screen)
2. **Track variables** - write down what each variable contains at each step
3. **Show iteration** - if it is a loop, show what happens in iteration 1, 2, etc.
4. **Explain as you go** - talk through your thinking out loud
5. **Arrive at the answer** - show what the final result is
6. **Handle errors gracefully** - if you make a mistake, correct it and keep going

**Example Whiteboarding Session:**
```
Code:
def add_numbers(lst):
    total = 0
    for num in lst:
        total = total + num
    return total

Call: add_numbers([5, 10, 3])

Whiteboard:
Step 1: total = 0, lst = [5, 10, 3]
Step 2 (Iteration 1): num = 5, total = 0 + 5 = 5
Step 3 (Iteration 2): num = 10, total = 5 + 10 = 15
Step 4 (Iteration 3): num = 3, total = 15 + 3 = 18
Step 5: return 18

Edge case - empty list:
Call: add_numbers([])
- Loop never executes
- total stays 0
- return 0
```

---

## How Questions Adapt During Code Review

The questions are not scripted - they adapt based on your responses:

- **If you trace perfectly** → You will move to edge case and modification questions
- **If you struggle with tracing** → We will focus more on execution before moving forward
- **If you get stuck** → We will ask clarifying questions to help you think through it

This means **you cannot memorize answers** - you need genuine understanding to do well.

---

✅ **DO:**
- Listen carefully to the question
- Take a moment to think before answering
- Ask for clarification if you do not understand
- Show your work on the whiteboard step-by-step
- Admit if you are unsure about something
- Point to your code for reference

❌ **DO NOT:**
- Rush to answer
- Make up answers
- Defend code you do not understand
- Ignore the question and explain something else
- Get defensive about feedback

---

## After Code Review

**Regardless of approval:**
- Thank your TL for feedback
- Ask for clarification on any suggestions
- Take notes on areas to improve
- Implement requested changes

---

**Remember:** Code reviews are not about being perfect. They are about demonstrating that you understand the code you wrote. We want to see that you can trace through your own code and explain what is happening! 
