# Code Review Preparation Guide

## What to Expect During Code Review

**Duration:** ~30 minutes per PR  
**Audience:** You + Teaching Assistant/Instructor  
**Format:**
1. TL reviews your code on screen (~10 min)
2. TL asks conceptual questions (~15 min)
3. You may be asked to whiteboard solutions (~5 min)

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

## Conceptual Questions Bank

The TL may ask questions from these categories. **Study these and be prepared!**

### 1. Object-Oriented Programming (OOP)

#### Class Design & Responsibility
- "Why did you create separate classes for X and Y?"
- "What is the single responsibility of this class?"
- "How would you refactor this code to follow OOP principles?"
- "Draw me a diagram showing how your classes interact"
- "Could you combine these two classes? Why/why not?"
- "What would break if you moved this method to a different class?"

#### Encapsulation & Data Hiding
- "Why do you have this attribute? Could it be private?"
- "What attributes does your class need to expose?"
- "How does your class protect its internal state?"
- "If someone uses your class wrong, how does it fail?"

#### Inheritance & Composition
- "Do your classes share behavior? Should they inherit from a parent class?"
- "When would you use inheritance vs composition?"
- "What if you had to add a third class? How would it fit?"

#### Method Design
- "This method does too much. How would you break it into smaller methods?"
- "What would happen if someone passed None to this method?"
- "Why does this method return this specific type?"
- "Could this method have fewer parameters? How?"

### 2. Data Structures

#### Lists
- "Why did you choose a list for this instead of a dictionary?"
- "How do you handle duplicate items in your list?"
- "What's the complexity of finding an item in your list?"
- "How would you keep your list sorted?"

#### Dictionaries
- "What happens if the key doesn't exist in your dictionary?"
- "Why is a dictionary better than a list for this use case?"
- "Could you show me how you iterate over this dictionary?"
- "What if you needed to support multiple values per key?"

#### Complex Structures
- "Walk me through how you access nested data in this structure"
- "What validation do you do when adding to this data structure?"
- "How do you prevent corruption of this data?"

### 3. Error Handling & Validation

#### Input Validation
- "What happens if the user enters invalid input?"
- "How do you validate numeric input from users?"
- "Walk me through your validation logic for this function"
- "What edge cases did you consider for this input?"

#### Exception Handling
- "Why catch this specific exception instead of a general one?"
- "What happens if an exception occurs here and you don't catch it?"
- "Is it better to prevent an error or catch it?"
- "Show me a try/except block from your code and explain it"

#### Edge Cases
- "What happens if your list is empty?"
- "What if the user enters zero?"
- "What if a sensor read fails?"
- "How do you handle negative numbers/missing data/etc?"

### 4. Algorithms & Logic

#### Control Flow
- "Walk me through what this loop does step-by-step"
- "Why did you choose a while loop here instead of a for loop?"
- "What would happen if you removed this condition?"
- "Trace through this code with this example input"

#### Complexity & Efficiency
- "How many times does this loop execute in the worst case?"
- "Could you make this code faster? How?"
- "What's the time complexity of this operation?"

#### Correctness
- "Prove to me that this algorithm works correctly"
- "What test cases would you use for this function?"
- "Show me where a bug could hide in this code"

### 5. Design Patterns & Architecture

#### Code Organization
- "Why did you put this function in this class?"
- "How do you prevent code duplication?"
- "Show me an example of good separation of concerns in your code"
- "If you had to add a new feature, how would you organize it?"

#### Modularity
- "Could you reuse this class in another project?"
- "Are your methods too tightly coupled?"
- "How would you test this function in isolation?"

#### Configuration & Flexibility
- "What if you needed to change this hardcoded value?"
- "How would you make this code work with different inputs?"
- "What assumptions does your code make that might not always be true?"

### 6. Hardware Integration (if applicable)

#### Design
- "Why did you choose this specific hardware component?"
- "How does your code handle hardware failures?"
- "What happens if the hardware isn't connected?"
- "How would you add support for a second sensor?"

#### Debugging
- "How do you test your hardware code?"
- "What's the most common hardware failure you've handled?"
- "Show me your error handling for hardware operations"

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
