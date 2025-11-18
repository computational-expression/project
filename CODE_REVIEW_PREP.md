# Code Review Preparation Guide

## What to Expect During Code Review

**Duration:** ~30 minutes per PR  
**Audience:** You + Teaching Assistant/Instructor  
**Format:**
1. TL reviews your code on screen (~10 min)
2. TL asks conceptual questions from our slides (~15 min)
3. You may be asked to whiteboard solutions (~5 min)

**How Conceptual Questions Work:**
- We will **randomly select 3 concepts** from the list below
- Each concept is something we covered in lectures (Weeks 2-12)
- You should be able to explain how you used each concept in YOUR code
- Questions will ask about the "how" and "why" of your implementation
- No trick questions - just checking your understanding!

---

## Before Your Code Review

### Prepare Your Code
- [ ] Code is clean and well-commented
- [ ] All docstrings are complete and accurate
- [ ] Code runs without errors
- [ ] You've tested all major features
- [ ] No unused imports or variables

### Know Your Code
- [ ] Understand every line you wrote
- [ ] Be able to explain why you made design choices
- [ ] Know the flow of your main functions
- [ ] Understand edge cases and error handling
- [ ] Be ready to modify code on the fly if asked

### Practice Whiteboarding
- [ ] Draw your class diagram
- [ ] Pseudocode your main algorithm
- [ ] Explain call flow between methods
- [ ] Show how data flows through your classes

### Prepare Examples
- [ ] Know how to run specific features
- [ ] Have test cases ready
- [ ] Know what inputs cause errors
- [ ] Be ready to show error handling

---

## Concepts We'll Ask About

During your code reviews, we will **randomly select 3 concepts** from this list to ask about. You should be prepared to explain how you used each concept in your code, how it works, and the trade-offs of your implementation.

**Study these concepts from our slides (Weeks 2-12):**

### Python Fundamentals (Week 2)
- **Variables & Naming** - Variable assignment, naming conventions, dynamic typing, scope
- **Program Structure** - Statements, indentation, code blocks, execution flow

### Data Types & Operations (Week 3)
- **Data Types** - int, float, str, bool, list, dict; type checking with `type()`
- **Operators** - Arithmetic (+, -, *, /, //, %), comparison (==, !=, <, >, <=, >=), logical (and, or, not), string concatenation/formatting

### Control Flow - Conditionals (Week 3)
- **If/Elif/Else** - Condition evaluation, boolean logic, nested conditionals, ternary operators

### Control Flow - Loops (Week 4)
- **For Loops** - Iteration over sequences, range(), loop variable usage, nested loops
- **While Loops** - Loop structure, exit conditions, infinite loop risks, loop counters

### Lists (Week 6)
- **List Operations** - Indexing, slicing, append, remove, insert, length, iteration
- **List Usage** - When to use lists, list methods, searching/filtering

### Dictionaries (Week 10)
- **Dictionary Structure** - Key-value pairs, accessing values, keys(), values(), items()
- **Dictionary Usage** - When to use dicts vs lists, nested structures, iteration patterns

### Functions & Methods (Week 9)
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

## Whiteboarding Exercise Examples

Be prepared to whiteboard solutions for questions like:

### Example 1: Class Diagram
**Question:** "Draw me a diagram showing your classes and how they interact"

**What to include:**
- Class boxes with attributes and methods
- Arrows showing relationships
- Labels showing what each class does

### Example 2: Function Trace
**Question:** "Trace through this function with input [X]"

**What to do:**
- Show variables at each step
- Show loop iterations
- Explain the final output

### Example 3: Pseudocode
**Question:** "Show me the pseudocode for your main algorithm"

**What to include:**
- High-level steps
- Decision points
- Loop structures
- Function calls

### Example 4: Error Handling
**Question:** "How would you handle a missing file error?"

**What to show:**
- Try/except block
- Specific exception to catch
- What happens in except block
- How user is informed

---

## Common Pitfall Answers to Avoid

❌ **BAD:** "I'm not sure... I just copied this from the internet"  
✅ **GOOD:** "I used this pattern because [reason]. Let me explain how it works..."

❌ **BAD:** "This is just how I wrote it"  
✅ **GOOD:** "I structured it this way because [design reasoning]..."

❌ **BAD:** "It works, so it must be right"  
✅ **GOOD:** "I tested it with these cases: [examples]. It handles these edge cases: [examples]..."

❌ **BAD:** "I don't know what my code does"  
✅ **GOOD:** "Line by line, this code does [explanation]..."

---

## How to Answer Questions

### Strategy 1: Explain Your Thinking
1. **Restate** the question to make sure you understand
2. **Explain** your approach and why you chose it
3. **Show** evidence (code, test results, logic)
4. **Defend** your choice with reasoning

**Example:**
> **Question:** "Why did you use a dictionary here instead of a list?"  
> **Answer:** "I used a dictionary because I need to look up items by their name, not by position. If I used a list, I'd have to search through every element to find the right one. With a dictionary, lookup is O(1) instead of O(n)."

### Strategy 2: Show Your Code
1. **Point to** the relevant code on screen
2. **Read** the code out loud
3. **Explain** what each line does
4. **Show** an example execution

### Strategy 3: Use Examples
1. **Pick** a specific example input
2. **Trace** through your code with that input
3. **Show** the intermediate steps
4. **Arrive** at the correct output

### Strategy 4: Ask for Clarification
If you don't understand the question:
1. "Can you rephrase that?"
2. "Do you mean X or Y?"
3. "Can you show me an example?"

**Don't just guess!** It's better to ask than to answer wrongly.

---

## Red Flags That Show Lack of Understanding

🚩 You can't explain what your code does  
🚩 You don't know why you made a design choice  
🚩 You can't trace through your own code  
🚩 You can't explain an error your code throws  
🚩 You copy-pasted code without understanding it  
🚩 Your docstrings don't match what the code does  

---

## Green Flags That Show Understanding

✅ You can explain each design decision  
✅ You know edge cases your code handles  
✅ You can whiteboard your algorithm  
✅ You understand the trade-offs in your design  
✅ You can modify code on the fly  
✅ You can explain what happens if something fails  

---

## Practice Questions for Your Specific Project

Prepare answers for these (tailored to your project):

1. **Architecture Question:**
   "How do your classes interact in your main workflow?"

2. **Error Handling Question:**
   "What's the most important error your code needs to handle and how do you do it?"

3. **Data Structure Question:**
   "Show me your most important data structure and how you use it"

4. **Algorithm Question:**
   "Walk me through [your main function] step by step"

5. **Design Question:**
   "If you had to add [new feature], how would you change your design?"

---

## During Code Review: Tips

✅ **DO:**
- Listen carefully to the question
- Take a moment to think before answering
- Admit if you don't know something
- Ask for clarification if needed
- Back up claims with code/examples
- Be humble and ready to learn

❌ **DON'T:**
- Interrupt the TL
- Ramble without a clear answer
- Defend bad code decisions
- Blame external factors
- Guess or make things up
- Get defensive about feedback

---

## After Code Review

**Regardless of approval:**
- Thank your TL for feedback
- Take notes on improvement areas
- Ask clarifying questions if confused
- Implement requested changes promptly
- Learn from the feedback

---

## Practice Whiteboarding

**Before your code review, practice:**

1. **Draw your class diagram** on paper
2. **Whiteboard your main algorithm** with a friend
3. **Trace through code** with sample inputs
4. **Explain your design** out loud
5. **Answer practice questions** without looking at code

**Pro Tip:** Have a friend ask you questions while you whiteboard - it simulates the real experience!

---

**Remember:** Code reviews aren't about being perfect. They're about demonstrating understanding and being able to explain your work. The TL wants to see that you know what you built! 🎯
