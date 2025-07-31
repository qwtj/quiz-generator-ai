# AI Quiz Generator

This is a simple web application that uses an AI model to generate quizzes based on a given topic or URL.  It allows users to create multiple choice, write-in, and true/false questions, and provides features for importing and exporting quizzes as JSON files.

## Features

*   **Quiz Generation:**  Generates quizzes based on user-provided topics or URLs using the Gemini AI model.
*   **Question Types:** Supports multiple choice, write-in, and true/false question types.
*   **Import/Export:**  Allows users to import and export quizzes as JSON files for easy sharing and storage.
*   **Fact Checking:** Provides a fact-checking feature to validate the accuracy of quiz questions and answers.
*   **User Interface:** A clean and intuitive user interface for easy quiz creation and interaction.
*   **LaTeX Support:** Supports mathematical formulas using LaTeX formatting.
*   **Code Highlighting:** Supports code snippets with syntax highlighting.
*   **Accessibility:** Includes accessibility features such as ARIA labels and keyboard shortcuts for navigation.
*   **Share to X:** Easily share your quiz results on X (formerly Twitter).

## How to Use

1.  **Enter a Topic or URL:** In the text box at the top of the page, enter a topic or URL related to the quiz you want to generate (e.g., "5 questions on JavaScript").  Press Enter to submit.

2.  **Specify Question Types:** Use the action bar below the text box to add specific question types to your prompt.  Enter the number of questions you want for each type, then click the corresponding button (Multiple Choice, Write-In, True/False, Code).

3.  **Generate Quiz:** Click the "Generate Quiz" button to start the quiz generation process. The AI will generate questions based on your prompt.

4.  **Take the Quiz:** Once the quiz is generated, answer the questions.
    *   For multiple choice questions, click the option you think is correct. You can also use the `A`, `B`, `C`, and `D` keys to select options.
    *   For write-in questions, type your answer in the provided text box.

5.  **Fact Check:** After answering a question, a "Fact Check" button will appear. Click it to validate the question and answer.

6.  **View Results:** After completing the quiz, a results modal will display your score and a list of topics to review (if applicable).

7.  **Restart, Close, or Share:** You can restart the quiz, close the results modal, or share your results on X.

8.  **Import/Export:** Use the "import" command to upload a quiz from a JSON file or the "export" command to save the current quiz as a JSON file.

## Commands

You can type commands directly into the text box to perform specific actions:

*   `export`:  Downloads the current quiz as a JSON file.
*   `import`:  Opens a file dialog to load a quiz from a JSON file.

## Keyboard Shortcuts

*   When answering a multiple-choice quiz, you can use the following keys to select an answer:
    *   `A`
    *   `B`
    *   `C`
    *   `D`

## Technologies Used

*   HTML
*   CSS
*   JavaScript
*   Gemini API

## Setup/Installation

This project is a static HTML/CSS/JavaScript application.  No special installation steps are required. Simply open the `index.html` file in your web browser.

To use the Gemini API, you'll need an API key.  This is handled by the environment where the application is deployed and does not need to be configured in the code itself.  The `apiKey` variable in the JavaScript code should be left as an empty string:

```javascript
const apiKey = ""; // The environment will provide the key
```

## Important Notes

*   An API key is needed to use the Gemini AI model for quiz generation and grading. The environment where the application runs should provide the key.
*   The accuracy of the generated quiz questions and answers depends on the quality of the AI model.  Use the "Fact Check" feature to verify the information.
*   The application uses MathJax to render mathematical formulas.
*   The application utilizes Markdown parsing to render text, providing support for features such as code snippets with syntax highlighting, bold text, and italics.

