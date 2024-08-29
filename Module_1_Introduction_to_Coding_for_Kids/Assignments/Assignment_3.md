### Assignment: Design an Interactive Quiz Using Scratch

#### Problem Statement:
Create an interactive quiz in Scratch that tests coding knowledge based on the concepts learned in the lecture "Overview of Programming Languages for Kids." The quiz should engage kids aged 8-15 and include questions related to different programming languages, their features, and their applications in storytelling and game-based learning. This project will not only reinforce coding concepts but also enhance creativity and problem-solving skills among young learners.

#### Starter Code:
Below is a basic framework to help you get started with your interactive quiz in Scratch. You will need to create sprites for the questions and answers, as well as add scripts to handle user interactions.

```scratch
// Starter code for interactive quiz in Scratch

// When the green flag is clicked, start the quiz
when green flag clicked
set [score v] to [0] // Initialize score
ask [What is the main purpose of Scratch?] and wait // Ask the first question

// Check the answer
if <(answer) = [To create animations and games]> then
    change [score v] by (1) // Increment score if correct
    say [Correct! Well done!] for (2) seconds
else
    say [Oops! That's not right. Try again!] for (2) seconds
end

// Continue with more questions...
ask [What programming language is known for its simplicity?] and wait
if <(answer) = [Python]> then
    change [score v] by (1)
    say [Correct! Python is great for beginners.] for (2) seconds
else
    say [Not quite! The answer is Python.] for (2) seconds
end

// Display final score at the end of the quiz
say (join [Your final score is: ] (score)) for (5) seconds
```

#### Detailed Instructions:
1. **Set Up Your Scratch Project**:
   - Open Scratch and create a new project.
   - Add a backdrop that relates to coding or education to make it visually appealing.

2. **Create Sprites**:
   - Design or select sprites for the quiz master (who will ask questions) and for each answer option.
   - Optionally, create a score display sprite to show the user's score.

3. **Add Questions**:
   - Use the `ask` block to present multiple questions about programming languages, their uses, and benefits.
   - Ensure each question has a correct answer and at least two incorrect options.

4. **Handle User Input**:
   - Use conditional statements (`if` blocks) to check if the user's answer is correct.
   - Provide feedback using `say` blocks based on whether the answer was right or wrong.

5. **Score Keeping**:
   - Implement a variable called `score` to keep track of the number of correct answers.
   - Display the final score at the end of the quiz using a `say` block.

6. **Enhancements**:
   - Consider adding features such as a timer for each question or lifelines (like hints) to make the quiz more engaging.
   - You could also include fun facts about programming languages after each question to enrich learning.

#### Criteria for Success and Evaluation:
- **Functionality**: The quiz should run smoothly without errors, and all questions should be answerable.
- **Engagement**: The design should be visually appealing and engaging for kids aged 8-15.
- **Educational Value**: The questions should accurately reflect the concepts discussed in the lecture, enhancing the learner's knowledge of coding.
- **Code Quality**: Ensure that your Scratch code is well-organized, with clear labels and comments where necessary.

**Success Criteria**:
- The quiz correctly assesses knowledge of programming languages.
- The score is calculated accurately based on user responses.
- The project is interactive and encourages learning through engagement.

This assignment will help you build a portfolio of educational coding projects that you can teach to kids, aligning with your career goals in EdTech. Enjoy creating your interactive quiz!