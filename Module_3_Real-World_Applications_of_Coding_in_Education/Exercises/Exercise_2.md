# Module Title: Real-World Applications of Coding in Education

## Exercise Requirements

### 1. Problem Statement
You are tasked with building a weather reporting tool that not only displays the current weather but also incorporates basic mathematical calculations to enhance the user experience. The tool should allow users to input temperature in Celsius and convert it to Fahrenheit. Additionally, it should calculate the average temperature over a week based on user inputs. This exercise will require you to apply the mathematical concepts discussed in the lecture, such as basic arithmetic operations and functions.

### 2. Fill-in-the-Blank Starter Code
Below is the starter code for your weather reporting tool. Fill in the blanks to complete the functionality of the program.

```python
# Starter code for a weather reporting tool

def celsius_to_fahrenheit(celsius):
    # Convert Celsius to Fahrenheit using the formula (C * 9/5) + 32
    fahrenheit = _______ * _______ + _______
    return fahrenheit

def calculate_average_temperature(temperatures):
    # Calculate the average temperature from a list of temperatures
    total = 0
    for temp in temperatures:
        total += temp  # Sum all temperatures
    average = total / len(temperatures)  # Divide by the number of temperatures
    return average

# Example usage
week_temperatures = [15, 20, 18, 22, 19, 25, 21]  # Temperatures for a week in Celsius
average_temp = calculate_average_temperature(week_temperatures)
print("Average Temperature (Celsius):", average_temp)
print("Average Temperature (Fahrenheit):", celsius_to_fahrenheit(average_temp))
```

### 3. Hints
- For the `celsius_to_fahrenheit` function, remember the formula for converting Celsius to Fahrenheit: \( F = C \times \frac{9}{5} + 32 \). Think about what values you need to plug into the formula.
- In the `calculate_average_temperature` function, ensure that you are correctly summing the temperatures and dividing by the count of temperatures. Use `len(temperatures)` to get the number of temperature entries.
- Make sure to include error handling in your final solution. For example, check if the list of temperatures is empty before calculating the average.

### 4. Expected Outcome
By completing this exercise, you should be able to:
- Correctly fill in the blanks in the provided starter code.
- Demonstrate an understanding of how basic arithmetic operations apply to real-world scenarios, such as temperature conversion and averaging.
- Create a functional weather reporting tool that showcases your ability to integrate mathematical concepts into coding projects for kids aged 8-15.
- Ensure your final solution is well-commented, explaining the reasoning behind each step and adhering to best practices in coding.

---

This exercise is designed to promote critical thinking and application of mathematical concepts in programming while aligning with your goal of creating engaging educational content for kids. Happy coding!