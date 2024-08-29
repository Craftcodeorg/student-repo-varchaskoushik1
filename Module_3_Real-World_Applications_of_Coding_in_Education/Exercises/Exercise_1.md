# Module Title: Real-World Applications of Coding in Education

## Exercise Requirements

### 1. Problem Statement
You are tasked with creating a simple calculator application in Scratch that can help students understand basic math concepts while addressing a real-world problem. The calculator will allow users to perform addition, subtraction, multiplication, and division, and it should include a feature that helps them solve a problem related to budgeting for a community project. 

**Scenario**: Imagine your school wants to organize a community clean-up day. Students need to calculate how much money they will need for supplies based on the number of volunteers and the estimated cost per supply item. Your calculator will help them input the number of volunteers and the cost per supply item to get the total budget needed for the event.

### 2. Fill-in-the-Blank Starter Code
Below is a starter code snippet for your Scratch calculator project. You will need to fill in the blanks to complete the functionality of the calculator. Each blank corresponds to a specific coding concept discussed in the lecture.

```scratch
// Starter code for the calculator application
when green flag clicked
set [numberOfVolunteers v] to (0) // Input for number of volunteers
set [costPerSupply v] to (0) // Input for cost per supply item
set [totalBudget v] to (0) // Variable to store total budget

// Function to calculate total budget
define calculateBudget
    // Calculate total budget by multiplying number of volunteers by cost per supply
    set [totalBudget v] to (_______ * _______)
    say (join [Total Budget Needed: ] (totalBudget)) for (2) seconds

// Call the function when user inputs values
when [calculate v] clicked
    ask [Enter number of volunteers:] and wait
    set [numberOfVolunteers v] to (answer)
    ask [Enter cost per supply item:] and wait
    set [costPerSupply v] to (answer)
    calculateBudget
```

### 3. Hints
- **Hint 1**: Remember that in Scratch, you can use the multiplication operator (*) to perform calculations. Think about how you can multiply the number of volunteers by the cost per supply.
- **Hint 2**: Ensure that you are using the correct variable names when filling in the blanks. The variables you defined at the beginning of your code will help you store and manipulate user inputs.
- **Hint 3**: After calculating the total budget, use the `say` block to display the result to the user. This reinforces the storytelling aspect by providing immediate feedback.

### 4. Expected Outcome
By completing this exercise, you should be able to:
- Fill in the blanks correctly, demonstrating an understanding of how multiplication can solve real-world budgeting problems.
- Create a functional Scratch calculator that engages students in practical math applications.
- Provide clear feedback using Scratch's `say` block, enhancing the storytelling aspect of your project.

The final solution should adhere to best practices in coding and include comments that explain each step clearly, reinforcing the concepts discussed in the lecture. 

### Integration
This exercise is designed to be easily integrated into your learning platform, with clear headings and sections for easy navigation. Use markdown formatting for clarity, and ensure that all resources are linked appropriately for student access.