# Quizzler - A Python Trivia Game

Quizzler is a simple trivia game built using Python and Tkinter. It presents the user with a series of true/false questions and tracks their score as they progress through the game.

## Features

- **Interactive Interface**: Users can interact with the game through a graphical user interface (GUI) built using Tkinter.
- **Trivia Questions**: The game presents a series of true/false questions sourced from an API.
- **Score Tracking**: The user's score is displayed on the interface, updating as they answer questions.
- **Feedback**: Immediate feedback is provided to the user after answering each question, indicating whether their response was correct or incorrect.

## Requirements

- Python 3.x
- Tkinter (Python GUI library)

## Installation

1. Clone the repository:https://github.com/MihaiPopescu31/Quizz-App

2. Navigate to the project directory in your terminal or command prompt
  
3. Run the application:python main.py

## Code Explanation

In this section, we'll walk through the code step by step to understand how the Quizzler application works.

### `data.py`

This file handles the retrieval of trivia questions from the Open Trivia DB API. It defines parameters for the API request, sends the request, and stores the fetched questions in the `question_data` variable.

### `question.py`

Defines the `Question` class, representing a trivia question. Each question object has attributes `text` and `answer` to store the question and its correct answer, respectively.

### `quiz_brain.py`

Implements the `QuizBrain` class, which manages the game logic for Quizzler. It keeps track of the current question number, the user's score, and the list of trivia questions. It provides methods to check if there are more questions, retrieve the next question, and validate user answers.

### `ui.py`

Handles the graphical user interface (GUI) using Tkinter. It creates the main application window and components such as labels, buttons, and canvas to display questions and interact with the user. It utilizes the `QuizBrain` class to manage the game flow and update the GUI based on user input.

### Styling and Layout

The GUI elements are styled and laid out using Tkinter widgets and methods. The layout includes labels for the score and question, buttons for true/false answers, and a canvas for question display. Styling is applied using colors and images to enhance the user experience.

### Interaction and Flow

User interaction is managed through event-driven programming, where actions like button clicks trigger corresponding functions in the `QuizBrain` class. The application flow progresses as users answer questions, with feedback provided for correct and incorrect answers.

### Error Handling

The application incorporates error handling mechanisms to handle exceptions that may occur during API requests, data parsing, or user interactions. Error messages or warnings are displayed to the user when necessary, ensuring a smooth user experience.

### Conclusion

Together, these components form the Quizzler application, providing users with an engaging trivia quiz experience while demonstrating the use of APIs, object-oriented programming, and GUI development with Tkinter.

## How to Play
- **Launch the application.
- **Read each question presented on the screen.
- **Click the "True" or "False" button to answer each question.
- **Receive immediate feedback on your answer.
- **Continue answering questions until you reach the end of the quiz.



