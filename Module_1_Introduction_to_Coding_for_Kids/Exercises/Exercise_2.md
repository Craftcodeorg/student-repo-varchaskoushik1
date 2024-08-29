### Module Title: Introduction to Coding for Kids

### Exercise Requirements

#### 1. Problem Statement
Design a simple animation using loops in Scratch that tells a story about a character on an adventure. The character should move across the screen and perform actions based on user input. This exercise encourages students to apply their understanding of loops and storytelling in coding, fostering critical thinking and creativity as discussed in the lecture.

**Scenario**: Imagine a character named "Explorer Ellie" who is on a quest to find a hidden treasure. The students will create an animation where Ellie can move left or right based on user input, and they will use loops to make her walk continuously until the user decides to stop her.

#### 2. Fill-in-the-Blank Starter Code
Here’s a starter code snippet for Scratch. Students will fill in the blanks to complete the functionality of the animation.

```scratch
when green flag clicked
set [isWalking v] to [true]
forever
    if <(isWalking) = [true]> then
        move (10) steps
        wait (0.1) seconds
    end
end

when [space v] key pressed
    set [isWalking v] to [false]
    say [I found the treasure!] for (2) seconds
```

**Instructions for Students**:
- Fill in the blank for the number of steps Ellie should move when she walks.
- Explain how changing the wait time affects the speed of her movement.

#### 3. Hints
- **Hint 1**: Think about how you can control the speed of Ellie's movement. What happens if you increase or decrease the number of steps she takes?
- **Hint 2**: Remember that loops allow for repeated actions. How can you use this to make Ellie walk continuously until told to stop?
- **Hint 3**: Consider what happens when the space key is pressed. How does this action affect the animation?

#### 4. Expected Outcome
Students should successfully create an animation where Explorer Ellie moves across the screen continuously until the user presses the space key, at which point she stops and delivers a message about finding treasure. 

The final solution should:
- Use loops effectively to create continuous movement.
- Include comments explaining the purpose of each block of code.
- Demonstrate understanding of user input and its impact on animations.

### Integration
This exercise is structured with clear headings and sections for easy parsing and integration into your learning platform. The use of markdown formatting ensures clarity and accessibility for students. 

By completing this exercise, students will not only practice their coding skills but also enhance their storytelling abilities through interactive programming, aligning perfectly with your goals of creating captivating educational experiences for kids aged 8-15.