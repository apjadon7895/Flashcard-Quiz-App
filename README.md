# Quiz App

This project is a simple **Quiz Application** built using **React.js**. Users can answer multiple-choice questions and view their scores at the end. The app allows users to retry the quiz after viewing their results.

## Features

- **Multiple-Choice Questions:** The quiz consists of multiple questions with several answer options. 
- **Score Calculation:** The app keeps track of the user’s score as they answer each question.
- **Try Again:** After completing the quiz, the user can view their score and reset the quiz to try again.

## Components

### 1. `Quiz`
This is the main component that handles the quiz logic. It keeps track of the current question, user score, and whether the quiz has ended.

- **State Variables**:
  - `currentQuestion`: Tracks the index of the current question being displayed.
  - `score`: Tracks the number of correct answers.
  - `clickedOption`: Tracks the option selected by the user.
  - `showResult`: Tracks whether the quiz has ended and shows the result.

- **Functions**:
  - `changeQuestion`: Advances to the next question and updates the score.
  - `updateScore`: Increases the score if the correct option is selected.
  - `resetAll`: Resets the quiz to the initial state, allowing the user to retry.

### 2. `QuizResult`
This component displays the user's score and gives an option to retry the quiz.

- **Props**:
  - `score`: The user's score.
  - `totalScore`: The total number of questions in the quiz.
  - `tryAgain`: The function to reset the quiz.

## Data

The questions are imported from the `QuizData` object located in the `Data/QuizData.js` file. Each question contains:

- `question`: The text of the question.
- `options`: An array of possible answers.
- `answer`: The correct answer (an integer representing the index of the correct option).


