# Assignment: Develop a Mini-Game Incorporating Math Problems

## Problem Statement
Create an engaging mini-game designed for kids aged 8-15 that incorporates math problems for players to solve. The game should challenge players with various math problems that they need to answer correctly to progress through different levels. This assignment will help students apply the concepts of coding, critical thinking, and creativity discussed in the lecture "Importance of Coding in Education." The game should also include elements of storytelling to enhance engagement.

## Starter Code
Below is a basic framework for your mini-game using Python. This code sets up the game and includes comments to guide you on where to implement your solutions.

```python
import random

def start_game():
    print("Welcome to the Math Adventure Game!")
    print("Solve math problems to move forward in your adventure.")
    level = 1
    while level <= 5:  # 5 levels of increasing difficulty
        print(f"\nLevel {level}")
        if not play_level(level):
            print("Game Over! Try again.")
            return
        level += 1
    print("Congratulations! You've completed the Math Adventure!")

def play_level(level):
    # Generate math problems based on the current level
    correct_answers = 0
    total_questions = 3  # Number of questions per level

    for _ in range(total_questions):
        num1 = random.randint(1, 10 * level)
        num2 = random.randint(1, 10 * level)
        operation = random.choice(['+', '-', '*', '/'])
        
        if operation == '+':
            answer = num1 + num2
        elif operation == '-':
            answer = num1 - num2
        elif operation == '*':
            answer = num1 * num2
        else:
            answer = round(num1 / num2, 2)  # Round division to 2 decimal places

        user_answer = float(input(f"What is {num1} {operation} {num2}? "))
        
        if user_answer == answer:
            print("Correct!")
            correct_answers += 1
        else:
            print(f"Wrong! The correct answer is {answer}.")

    return correct_answers == total_questions

# Start the game
start_game()
```

## Detailed Instructions
1. **Level Design**: Modify the `play_level` function to introduce different types of math problems based on the level. For example, in level 1, use simple addition and subtraction. As levels increase, incorporate multiplication and division.

2. **Storytelling Elements**: Add a narrative that progresses with each level. For instance, after completing each level, include a short story segment that describes what happens next in the adventure. You can use print statements to narrate these segments.

3. **User Feedback**: Enhance user feedback by providing hints for incorrect answers. For example, if a player answers incorrectly, you could offer a hint related to the math operation being performed.

4. **Scoring System**: Implement a scoring system that tracks the number of correct answers and displays the score at the end of the game. You can add a congratulatory message based on the final score.

5. **Game Restart Option**: After completing the game, give players an option to restart or exit. This can be done using an input prompt asking if they want to play again.

## Criteria for Success and Evaluation
- **Functionality**: The game should run without errors and allow players to progress through levels by solving math problems.
- **Engagement**: The integration of storytelling elements should enhance player engagement throughout the game.
- **User Experience**: The game should provide clear instructions and feedback, making it easy for kids to understand how to play.
- **Code Quality**: The code should be clean, well-documented, and follow best practices for readability and maintainability.

### Success Criteria:
- The game correctly generates math problems appropriate for each level.
- The narrative progresses logically with each level completed.
- User feedback is informative and helps players learn from their mistakes.
- The code adheres to Python coding standards and is easy to follow.

By completing this assignment, you will gain hands-on experience in creating educational games that not only teach coding skills but also promote math learning in a fun and interactive way. Good luck!