# TestCaseGeneration

This repository provides a Python-based application to generate test cases and test artifacts for the Q&A team. It uses OpenAI's GPT-4 model to create detailed and structured test documentation based on software requirements.

## Features

- **Test Case Generation**: Automatically generate functional, edge, and negative test cases based on a given software requirement.
- **Test Artifact Generation**: Create test plans, user scenarios, and sample test data in Markdown format.
- **Customizable Prompts**: Easily modify the prompt templates to suit your specific needs.
- **File Saving**: Save generated test cases and artifacts to files for easy sharing and documentation.

## Prerequisites

- Python 3.7 or higher
- OpenAI API key
- Required Python packages (see [Installation](#installation))

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/your-username/TestCaseGeneration.git
   cd TestCaseGeneration
   ```

2. Install the required dependencies:

   ```bash
   pip install -r requirements.txt
   ```

3. Set up your OpenAI API key:
   - Create a `.env` file in the root directory.
   - Add the following line to the `.env` file:
     ```
     OPENAI_API_KEY=your_openai_api_key
     ```

## Usage

1. Edit the

requirement_text

variable in

TestCase.py

to include your software requirement.

2. Run the script:

   ```bash
   python TestCase.py
   ```

3. The generated test cases and artifacts will be saved as test_cases.txt and
   test_artifacts.md in the project directory.

## Example

### Input Requirement

```
Implement a login functionality where users enter their email and password.
If the credentials are correct, they are redirected to the dashboard.
If incorrect, an error message is displayed.
```

### Generated Output

#### Test Cases

```
Test Case ID: TC-001
Description: Verify login with valid credentials.
Steps:
1. Enter a valid email and password.
2. Click the login button.
Expected Result: User is redirected to the dashboard.
```

#### Test Artifacts

- **Test Plan**: Objectives, scope, and responsibilities.
- **User Scenarios**: Realistic user interactions with the system.
- **Test Data**: Sample test data for testing.

## Contributing

Contributions are welcome! Feel free to open issues or submit pull requests to improve this project.

## License

This project is licensed under the MIT License. See the LICENSE file for details.

## Acknowledgments

- [LangChain](https://github.com/hwchase17/langchain) for prompt templates.
- OpenAI for the GPT-4 model.

```

```
