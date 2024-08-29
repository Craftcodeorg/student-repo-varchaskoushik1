### Module Title: Learning Experience Design for Kids

### Exercise Requirements

#### 1. Problem Statement
Create an interactive quiz that incorporates storytelling elements to engage kids aged 8-15 in learning coding concepts. The quiz should consist of a narrative that unfolds as the student progresses through the questions, with each question presenting a challenge that relates to the story. For example, a story about a young coder who must solve coding puzzles to save their digital kingdom from a bug invasion.

#### 2. Fill-in-the-Blank Starter Code
Below is a starter code template for creating an interactive quiz using Python. Fill in the blanks to complete the functionality of the quiz.

```python
# Starter code for implementing storytelling in an interactive quiz
def interactive_quiz():
    score = 0  # Initialize score
    print("Welcome to the Coding Adventure Quiz!")
    print("You are a young coder trying to save your digital kingdom from bugs.")
    
    # Question 1
    answer1 = input("What does 'print' do in Python? (a) Displays output (b) Saves data\n")
    if answer1.lower() == 'a':
        print("Correct! You've defeated the first bug!")
        score += 1
    else:
        print("Oops! That's not right. The correct answer is (a) Displays output.")
    
    # Question 2
    answer2 = input("What symbol is used for comments in Python? (a) // (b) #\n")
    if answer2.lower() == 'b':
        print("Great job! You've vanquished another bug!")
        score += 1
    else:
        print("Not quite! The correct answer is (b) #.")
    
    # Final score
    print(f"Your final score is: {score} out of 2")
    
# Call the function to run the quiz
interactive_quiz()
```

#### 3. Hints
- **Hint for Question 1**: Think about how you display information on the screen when coding. What command would you use?
- **Hint for Question 2**: Remember that comments are used to leave notes in your code. Which symbol is commonly used in Python to indicate comments?
- **General Hint**: Use storytelling to make each question feel like a part of the adventure. Consider adding more questions that relate to different coding concepts.

#### 4. Expected Outcome
The student should be able to fill in the blanks correctly, demonstrating their understanding of how storytelling can enhance engagement in educational content. The completed quiz should:
- Present a narrative that captivates kids and encourages them to participate.
- Include at least two questions related to coding concepts.
- Maintain a scoring system that provides feedback based on the answers given.
- Be well-commented, explaining the purpose of each part of the code and how it relates to storytelling and coding education.

### Integration
This exercise is structured to facilitate easy integration into an EdTech learning platform. Each section is clearly labeled, and the use of markdown formatting ensures readability. The exercise encourages project-based learning and interactive engagement, aligning with the user's preferences and career goals in teaching coding for kids.