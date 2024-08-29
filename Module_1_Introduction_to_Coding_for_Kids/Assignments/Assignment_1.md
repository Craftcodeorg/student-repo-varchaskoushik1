# Assignment: Create a Scratch Project that Tells a Story Using Characters and Scenes

## Problem Statement:
You are tasked with creating an interactive story using Scratch, a visual programming language designed for kids. Your project should incorporate the key coding concepts discussed in the lecture, such as algorithms and variables, to enhance the storytelling experience. The story should allow users to make choices that affect the outcome, demonstrating how coding can be used to create engaging narratives.

## Starter Code:
While Scratch uses a block-based interface rather than traditional coding, here’s a conceptual outline of how you might structure your project. You will need to create sprites (characters) and backdrops (scenes) in Scratch. Below is a description of how you might set up your project:

1. **Create Sprites**: 
   - A character sprite (e.g., a hero).
   - A choice sprite (e.g., a question mark).
   - Background sprites for different scenes.

2. **Setup Backdrops**: 
   - Create multiple backdrops representing different scenes in your story.

3. **Basic Logic**: 
   - Use the following pseudocode as a guideline to implement your logic in Scratch:

```plaintext
START
SET userChoice = ""
SHOW characterSprite ON backdrop1

IF user clicks on choiceSprite THEN
    userChoice = user’s selection (e.g., "Explore" or "Stay")
    
    IF userChoice == "Explore" THEN
        SWITCH backdrop to backdrop2
        SHOW next part of the story
    ELSE
        SWITCH backdrop to backdrop3
        SHOW alternative part of the story
    END IF
END IF
```

## Detailed Instructions:
1. **Create Your Sprites**:
   - In Scratch, create or choose your character sprite that will be the main character of your story.
   - Add additional sprites for choices or actions that the character can take.

2. **Design Your Backdrops**:
   - Create multiple backdrops that represent different parts of your story. For example, one backdrop could be a forest, and another could be a castle.

3. **Implement Basic Logic**:
   - Use the "when this sprite clicked" block to detect when a choice is made.
   - Use "if-else" blocks to determine what happens based on the user's choice.
   - Use "switch backdrop" blocks to change the scene according to the user's decisions.

4. **Add Variables**:
   - Create a variable called `userChoice` to store the user's selection.
   - Use this variable to determine which part of the story to show next.

5. **Enhance the Storytelling**:
   - Add dialogue or narration using text bubbles or sound clips.
   - Incorporate animations for your sprites to make the story more engaging.

## Criteria for Success and Evaluation:
Your project will be evaluated based on the following criteria:

- **Story Engagement**: The story should be interesting and engaging for kids aged 8-15.
- **Coding Concepts**: You should effectively use algorithms (if-else logic) and variables (userChoice) in your project.
- **User Interaction**: The project should allow users to make choices that affect the story’s outcome.
- **Creativity**: The overall creativity in storytelling, character design, and scene transitions will be assessed.
- **Technical Execution**: The project should run smoothly without errors, with clear instructions for users on how to interact with it.

By completing this assignment, you will not only apply the concepts learned in the lecture but also build a fun and educational project that you can share with kids, fulfilling your goal of creating captivating learning experiences in coding.