# CMPSC 100 - Final Project

## Overview

For this final project, you will develop a **Python application of your choice** that demonstrates your understanding of Python programming, and related programming concepts.

---

## Table of Contents

1. [Quick Start](#quick-start)
2. [Project Timeline](#project-timeline)
3. [Version Control Requirements](#version-control-requirements)
4. [Final Presentation](#final-presentation-december-8)
5. [File Structure](#file-structure)
6. [Tips for Success](#tips-for-success)

---

## Quick Start

**New to the project?** Follow these steps:

1. Read this README
2. Check `REQUIREMENTS.md` for complete checklist
3. Use templates in `src/` to start coding
4. Before code review, study `CODE_REVIEW_PREP.md`
5. Before presentation, review `PRESENTATION_RUBRIC.md`

---

## Project Timeline

| Date | Milestone | Description |
|------|-----------|-------------|
| **Nov 17 - Nov 24** | Design and Development Phase | Plan your application and finalize requirements. Start development of functionality. |
| **Nov 24 - Nov 25** | Development | Continue building core functionality |
| **Dec 1 - Dec 5** | Development | Submit two PRs for code review |
| **Dec 8** | Final Presentation | 5-minute overview presentation and live demo |

---

## Coding Requirements

**For complete details on all coding requirements, see `REQUIREMENTS.md`.**

The project requires:
- **Hardware projects:** Minimum 300 lines of code
- **Software-only projects:** Minimum 400 lines of code
- Minimum 2 classes with clear responsibilities
- At least 12 functions/methods total
- Error handling and edge case management
- Meaningful use of lists, dictionaries, and control flow
- A new hardware component OR new software concept
- Comprehensive docstrings and code documentation

---

## Version Control Requirements

### **Branch Strategy**
- **At least 2 separate branches** for feature development
- **Branch naming:** Use descriptive names
- **Main/Master branch:** Should remain stable; merges only via PR

### **Commit Messages**
- **Format:** Clear, descriptive messages that explain the "why" not just the "what"
- **Examples:**
  - ✅ `Add user authentication with password validation`
  - ✅ `Restructure database queries to reduce redundancy`
  - ✅ `Handle FileNotFoundError in data loader`
  - ❌ `fix bug`
  - ❌ `update code`
  - ❌ `changes`

### **Pull Requests**
- **Minimum 2 PRs:** Each PR should represent a logical feature or milestone
- **PR Descriptions:** Each PR must include:
  - Summary of changes
  - What problem it solves
  - How to test it
  - Any breaking changes or dependencies
  - Which assignment requirements it fulfills
- **Code Review:** Each PR must be reviewed and approved by a TL before merging

---

## Code Review Process (Week 15)

**For complete code review preparation details, see `CODE_REVIEW_PREP.md`.**

During your code reviews:
- TL will review your code and ask conceptual questions
- You'll explain design decisions and walk through key functions
- You may be asked to whiteboard algorithms or class diagrams
- Code must be cleaned, documented, and running without errors

**Prepare by:**
- Understanding every line you wrote
- Knowing why you made each design choice
- Testing all major features thoroughly
- Practicing explanations and whiteboarding

---

## Final Presentation (December 8)

### **Presentation Format**
- **Duration:** 5 minutes
- **Audience:** Entire class
- **Components:** Overview + Live Demo

### **What to Include**

**Overview (2-3 minutes):**
- What problem does your application solve?
- What are the key features?
- What hardware or new concept did you incorporate?
- Key design decisions and why you made them

**Live Demo (2 minutes):**
- Show your program running
- Demonstrate 2-3 key features
- Show how it handles an edge case or error gracefully
- Run it start to finish without errors

**See `PRESENTATION_RUBRIC.md` for the complete assessment checklist.**

---

## Grading

**Total Points: 15**

| Component | Points |
|-----------|--------|
| **Working Code** | 7 points |
| **Code Review #1** | 3 points |
| **Code Review #2** | 3 points |
| **Final Presentation** | 2 points |

---

## Using Resources & LLMs

**You are encouraged to use online resources and LLMs (including GitHub Copilot, ChatGPT, Claude, etc.) to help with your project.**

**However, there are important requirements:**

✅ **You must:**
- **Understand every line of code** you submit
- **Be able to explain** your code design and implementation
- **Be able to reproduce** any code you use (not just copy-paste)
- **Know why** you made each design choice
- **Be able to modify** your code if asked during code review

❌ **You cannot:**
- Submit code you don't understand
- Copy code without learning how it works
- Use AI-generated code that you can't explain in code review
- Claim code is yours if you can't discuss its implementation

**During code reviews**, you will be asked to explain your code and may be asked to:
- Trace through your functions with example inputs
- Whiteboard your algorithms
- Modify code on the fly
- Answer questions about design choices

If you can't explain or reproduce your code, that's a red flag that you haven't truly learned it.

**Bottom line:** Use resources to learn faster, but make sure the final code and understanding are genuinely yours.

---

### During Development
✅ Commit often with clear messages  
✅ Write docstrings as you code  
✅ Test edge cases early  
✅ Use meaningful variable names  
✅ Keep functions small and focused  

### Before Code Review
✅ Read all your code line-by-line  
✅ Understand why you made each design choice  
✅ Test with invalid inputs  
✅ Practice explaining your code  
✅ Be ready to whiteboard  

### During Code Review
✅ Listen to feedback carefully  
✅ Explain your thinking  
✅ Ask clarifying questions  
✅ Show code examples  
✅ Don't be defensive  

### Before Presentation
✅ Rehearse at least 3 times  
✅ Test your demo before class  
✅ Have backup plan if demo fails  
✅ Know your 2-3 key features  
✅ Practice handling questions  

---

## Common Mistakes to Avoid

❌ **Starting too late** - Start planning NOW  
❌ **Only one big commit** - Commit frequently!  
❌ **No error handling** - Test invalid inputs  
❌ **Copy-paste code** - Understand what you write  
❌ **Missing docstrings** - Document as you code  
❌ **Unclear PR descriptions** - Explain your changes  
❌ **Not practicing presentation** - Rehearse!  
❌ **Hardcoding values** - Use parameters instead  
❌ **No edge case testing** - What if list is empty?  
❌ **Vague commit messages** - "fix bug" tells nothing

---

## Git Workflow Example

```bash
# 1. Create and switch to feature branch
git checkout -b feature/core-functionality

# 2. Make changes and commit frequently
git add src/class1.py
git commit -m "Add User class with email validation"

git add src/class2.py
git commit -m "Add UserManager class with add/find methods"

# 3. Push branch to GitHub
git push origin feature/core-functionality

# 4. Create PR on GitHub
# - Write clear description of changes
# - Explain what problem it solves
# - Mention assignment requirements it fulfills

# 5. After TL approval, merge PR
git checkout main
git pull
git merge feature/core-functionality
git push origin main

# 6. Start second feature branch
git checkout -b feature/advanced-features
# ... repeat process
```

---

## Minimum Code Examples

### Minimum Data Structures
```python
# Lists (minimum 2)
users = ["alice", "bob", "charlie"]
scores = [95, 87, 92]

# Dictionaries (minimum 2)
user_profiles = {
    "alice": {"age": 20, "major": "CS"},
    "bob": {"age": 21, "major": "Math"}
}

config = {"max_attempts": 3, "timeout": 30}
```

### Minimum Control Flow
```python
# If/elif/else (minimum 8 if, 2 elif, 1 else)
if score > 90:
    grade = "A"
elif score > 80:
    grade = "B"
else:
    grade = "C"

# Loops (minimum 2 for, 1 while)
for user in users:
    print(user)

count = 0
while count < 10:
    count += 1
```

### Minimum Functions
```python
# Functions with parameters and return values
def calculate_gpa(scores):
    """Calculate GPA from list of scores."""
    return sum(scores) / len(scores)

def validate_input(user_input):
    """Validate and return cleaned input."""
    if not user_input:
        raise ValueError("Input cannot be empty")
    return user_input.strip().lower()

# Error handling
try:
    result = calculate_gpa([90, 85, 88])
except ZeroDivisionError:
    result = 0.0
```

### Minimum Classes
```python
class User:
    """Represents a user in the system."""
    def __init__(self, name, email):
        self.name = name
        self.email = email
    
    def update_email(self, new_email):
        """Update user's email address."""
        if "@" not in new_email:
            raise ValueError("Invalid email")
        self.email = new_email

class UserManager:
    """Manages a collection of users."""
    def __init__(self):
        self.users = {}
    
    def add_user(self, user):
        """Add a user to the system."""
        self.users[user.email] = user
    
    def find_user(self, email):
        """Find user by email."""
        return self.users.get(email, None)
```

---

## Resources

- **Lab Reference:** Look at labs 1-9 for code patterns
- **Python Docs:** https://docs.python.org/3/
- **Git Guide:** https://git-scm.com/book/en/v2
- **Markdown:** https://guides.github.com/features/mastering-markdown/

---

## Files in This Project

| File | Purpose |
|------|---------|
| `README.md` | Project overview and timeline |
| `REQUIREMENTS.md` | Complete checklist of all requirements |
| `CODE_REVIEW_PREP.md` | How to prepare for code review (week 15) |
| `PRESENTATION_RUBRIC.md` | How your presentation will be graded |
| `src/main.py` | Template for main entry point |
| `writing/report.md` | Template for your project report |

---

## Contact & Questions

For questions about the project:
- Read `REQUIREMENTS.md` for detailed information
- Check `CODE_REVIEW_PREP.md` if confused about code review
- Visit office hours for help
- Ask on the course forum

Good luck! 🚀
