# Assignment: Develop an Interactive Math Learning App for Kids

## Problem Statement
Create an interactive app that helps kids aged 8-15 learn math through engaging challenges. The app should focus on real-world math problems, allowing students to solve challenges that relate to everyday situations, such as budgeting for a party, calculating distances on a map, or determining the total cost of items while shopping. This project will enhance your storytelling skills by framing math problems in relatable narratives, making learning both fun and impactful.

## Starter Code
Below is a basic framework for the math learning app. The code sets up a simple command-line interface where kids can choose different math challenges to solve.

```python
# Starter code for the Interactive Math Learning App

def math_challenge():
    print("Welcome to the Math Learning App!")
    print("Choose a challenge:")
    print("1. Budgeting for a Party")
    print("2. Shopping Total Calculator")
    print("3. Distance Calculation")

    choice = input("Enter the number of your choice: ")

    if choice == '1':
        budgeting_challenge()
    elif choice == '2':
        shopping_challenge()
    elif choice == '3':
        distance_challenge()
    else:
        print("Invalid choice! Please select a valid challenge.")

def budgeting_challenge():
    budget = float(input("Enter your total budget for the party: "))
    cost_per_person = float(input("Enter the cost per person: "))
    num_people = int(input("Enter the number of people invited: "))
    
    total_cost = cost_per_person * num_people
    if total_cost <= budget:
        print(f"You can host the party! Total cost: ${total_cost:.2f}")
    else:
        print(f"Sorry, you need ${total_cost - budget:.2f} more to host the party.")

def shopping_challenge():
    item_count = int(input("How many items are you buying? "))
    total_cost = 0
    
    for i in range(item_count):
        price = float(input(f"Enter the price of item {i + 1}: $"))
        total_cost += price
    
    print(f"The total cost of your shopping is: ${total_cost:.2f}")

def distance_challenge():
    speed = float(input("Enter your speed in km/h: "))
    time = float(input("Enter time traveled in hours: "))
    
    distance = speed * time
    print(f"You will travel {distance:.2f} km.")

# Start the app
math_challenge()
```

## Detailed Instructions
1. **Challenge Selection**: Modify the `math_challenge()` function to include more engaging challenges or categories. Consider adding challenges related to geometry or time calculations.

2. **Enhance Budgeting Challenge**: 
   - Add a feature that allows users to input multiple costs (e.g., decorations, food, etc.) and calculate the total expenses.
   - Provide feedback on how much money is left after expenses.

3. **Improve Shopping Challenge**: 
   - Implement a discount feature where users can input a discount percentage and see the final price after applying the discount.
   - Allow users to input item names and quantities for better engagement.

4. **Expand Distance Challenge**: 
   - Include options for different modes of transportation (e.g., walking, biking, driving) with varying speeds.
   - Calculate estimated arrival times based on user input.

5. **User Interface**: 
   - Consider implementing a graphical user interface (GUI) using libraries like Tkinter or Pygame to make it more visually appealing for kids.
   - Add colorful graphics and sounds to enhance user engagement.

## Criteria for Success and Evaluation
- **Functionality**: The app must run without errors and provide accurate calculations based on user input.
- **User Engagement**: The challenges should be relatable and engaging for kids, encouraging them to think critically about math.
- **Code Quality**: The code should be well-structured, readable, and follow best practices (e.g., proper variable naming, comments).
- **Creativity**: The project should demonstrate creativity in how math concepts are presented and framed within real-world scenarios.

By completing this assignment, you will create an educational tool that not only teaches math but also engages kids through storytelling and real-life applications, aligning perfectly with your career goals in EdTech.