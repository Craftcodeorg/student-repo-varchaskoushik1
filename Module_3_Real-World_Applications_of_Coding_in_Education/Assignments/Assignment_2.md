# Assignment: Real-World Applications of Coding in Education

## Problem Statement
Create a project that combines real-world weather data with coding skills to teach kids aged 8-15 about data analysis and visualization. The project will involve creating a simple Python program that fetches weather data from an API, processes this data using basic arithmetic, and visualizes the results in a user-friendly format. This task will help students understand how math and programming work together to analyze real-world information.

## Starter Code
Below is the starter code that sets up the environment for the project. This code includes comments to guide you on where to implement your solutions.

```python
import requests
import matplotlib.pyplot as plt

def fetch_weather_data(city):
    # Step 1: Fetch weather data from an API (OpenWeatherMap)
    api_key = 'YOUR_API_KEY'  # Replace with your OpenWeatherMap API key
    url = f'http://api.openweathermap.org/data/2.5/weather?q={city}&appid={api_key}&units=metric'
    
    response = requests.get(url)
    if response.status_code == 200:
        return response.json()
    else:
        print("Error fetching data.")
        return None

def analyze_weather_data(data):
    # Step 2: Extract relevant information from the weather data
    temperature = data['main']['temp']
    humidity = data['main']['humidity']
    
    # Step 3: Perform basic arithmetic to analyze the data
    feels_like = temperature + ((humidity / 100) * 10)  # Simplified 'feels like' calculation
    
    return temperature, humidity, feels_like

def visualize_weather_data(city, temperature, humidity, feels_like):
    # Step 4: Visualize the weather data using a bar chart
    labels = ['Temperature (°C)', 'Humidity (%)', 'Feels Like (°C)']
    values = [temperature, humidity, feels_like]
    
    plt.bar(labels, values, color=['blue', 'green', 'orange'])
    plt.title(f'Weather Data for {city}')
    plt.ylabel('Values')
    plt.show()

# Test the functions with a sample city
city = 'London'
weather_data = fetch_weather_data(city)
if weather_data:
    temperature, humidity, feels_like = analyze_weather_data(weather_data)
    visualize_weather_data(city, temperature, humidity, feels_like)
```

## Detailed Instructions
1. **Step 1**: Replace `'YOUR_API_KEY'` with your actual OpenWeatherMap API key. You can sign up for a free account to obtain one.

2. **Step 2**: Modify the `analyze_weather_data` function to include additional calculations:
   - Calculate the difference between the current temperature and a predefined comfortable temperature (e.g., 22°C).
   - Return this difference along with the existing values.

3. **Step 3**: Enhance the `visualize_weather_data` function to include a label for the new calculated difference in temperature. You can add this as another bar in the chart.

4. **Step 4**: Add error handling in the `fetch_weather_data` function to manage cases where the city is not found or the API request fails.

5. **Step 5**: Create a simple user interface (UI) where kids can input their city name and get real-time weather updates. You can use `input()` to get user input from the console.

## Criteria for Success and Evaluation
**Success Criteria**:
- The program successfully fetches weather data from the API and handles errors appropriately.
- The `analyze_weather_data` function correctly computes and returns all required values.
- The `visualize_weather_data` function displays a clear and informative bar chart.
- The code is clean, well-documented with comments, and follows best practices for readability.
- The user interface allows kids to easily input their city and receive feedback.

### Evaluation Rubric:
- **Functionality (40%)**: Does the program run without errors? Does it fetch and display correct weather data?
- **Code Quality (30%)**: Is the code well-organized, readable, and documented?
- **User Experience (20%)**: Is the user interface intuitive and easy for kids to use?
- **Creativity (10%)**: Are there any additional features or enhancements that improve the project?

This assignment is designed to reinforce key concepts from the lecture while providing a fun and engaging way for students to apply their coding skills in a real-world context relevant to EdTech.