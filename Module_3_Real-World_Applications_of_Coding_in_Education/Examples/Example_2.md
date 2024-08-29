# Module Title: Real-World Applications of Coding in Education

## Example 2: Creating a Weather App Using Coding Concepts

### 1. Introduction
Creating a weather app is an excellent way to demonstrate the practical applications of coding concepts covered in the lecture "The Role of Math in Programming Concepts." This project not only engages students but also allows them to see how mathematical principles are essential in real-world applications. By developing a weather app, learners can apply their understanding of variables, data types, arithmetic operations, and logic in a meaningful way that resonates with everyday life.

### 2. Code Snippet
Here’s a simple weather app that fetches weather data from an API and displays it to the user. This code is suitable for intermediate-level programmers and includes error handling and best practices.

```python
import requests

def get_weather(city):
    """
    Fetches weather data for a specified city from the OpenWeatherMap API.
    
    Parameters:
    city (str): The name of the city for which to fetch weather data.
    
    Returns:
    dict: A dictionary containing weather information or an error message.
    """
    api_key = 'YOUR_API_KEY'  # Replace with your OpenWeatherMap API key
    base_url = f"http://api.openweathermap.org/data/2.5/weather?q={city}&appid={api_key}&units=metric"
    
    try:
        response = requests.get(base_url)
        response.raise_for_status()  # Raise an error for bad responses (4xx or 5xx)
        
        weather_data = response.json()
        
        if 'main' in weather_data:
            temperature = weather_data['main']['temp']
            description = weather_data['weather'][0]['description']
            return {
                'temperature': temperature,
                'description': description,
                'city': city
            }
        else:
            return {'error': 'Weather data not found for the specified city.'}
    
    except requests.exceptions.HTTPError as http_err:
        return {'error': f'HTTP error occurred: {http_err}'}
    except Exception as err:
        return {'error': f'An error occurred: {err}'}

# Example usage
city_name = input("Enter city name: ")
weather_info = get_weather(city_name)

if 'error' in weather_info:
    print(weather_info['error'])
else:
    print(f"Weather in {weather_info['city']}:")
    print(f"Temperature: {weather_info['temperature']}°C")
    print(f"Description: {weather_info['description']}")
```

### 3. Explanation
- **Importing Libraries**: The code begins by importing the `requests` library, which is essential for making HTTP requests to APIs.
  
- **Function Definition**: The `get_weather` function takes a city name as input and constructs the API URL using the OpenWeatherMap service. It incorporates error handling to manage potential issues with the API call.

- **API Call**: The function uses `requests.get()` to fetch data from the API. The `raise_for_status()` method checks for HTTP errors, ensuring that the program can handle issues gracefully.

- **Data Extraction**: If the response is successful, the function extracts temperature and weather description from the JSON response. This demonstrates the use of variables and data types as discussed in the lecture.

- **Error Handling**: The code includes comprehensive error handling for both HTTP errors and general exceptions, ensuring robustness.

- **User Interaction**: The example usage prompts the user to enter a city name, showcasing how user input can drive functionality in coding projects.

### 4. Application
The development of a weather app illustrates several key concepts relevant to EdTech:
- **Engagement**: By building a project that students can relate to, such as checking the weather, educators can enhance student engagement and interest in coding.
  
- **Real-World Relevance**: This application connects coding concepts with real-world scenarios, helping students understand how coding can solve everyday problems.

- **Skill Development**: Students learn to work with APIs, manage data, and implement error handling—skills that are crucial in both programming and practical applications in technology.

- **Cross-Disciplinary Learning**: The project integrates math (for calculations related to temperature conversion) and science (understanding weather patterns), fostering a holistic learning experience.

### Integration
This content is structured with clear headings and sections for easy parsing and integration into your learning platform. Each section builds upon the previous one, reinforcing key concepts while providing practical applications relevant to your goals of teaching coding to kids aged 8-15. By implementing projects like this weather app, you can create captivating learning experiences that not only teach coding but also inspire creativity and problem-solving among your students.