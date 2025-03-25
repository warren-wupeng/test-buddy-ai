# test-buddy-ai

# TestBuddyAI

**TestBuddyAI** is an AI-powered testing assistant designed for programmers. It automatically generates test cases, runs tests, and reports issues for your code repository—all running locally via Docker. Whether you're working on a personal project or a team codebase, TestBuddyAI helps you improve code quality and test coverage effortlessly.

---

## Features

- **Automated Test Generation**: Analyzes your code and generates unit/integration tests using advanced AI.
- **Continuous Testing**: Monitors code changes, runs tests, and keeps your test suite up-to-date.
- **Issue Reporting**: Identifies test failures, bugs, and low-coverage areas with actionable suggestions.
- **Local Execution**: Runs entirely on your machine via Docker, ensuring privacy and control.
- **Simple Interface**: A minimal React frontend to view test results and manage configurations.

---

## Tech Stack

- **Frontend**: React
- **Backend**: FastAPI
- **AI**: Large Language Model (LLM) + Retrieval-Augmented Generation (RAG)
- **Testing**: pytest
- **Containerization**: Docker

---

## Getting Started

### Prerequisites
- Docker installed on your machine
- A local code repository to test

### Installation
1. **Clone the Repository**
```bash
   git clone https://github.com/your-username/TestBuddyAI.git
   cd TestBuddyAI
```
2. Build and Run with Docker
```bash

docker build -t testbuddyai .
docker run -v /path/to/your/repo:/app/repo -p 3000:3000 -p 8000:8000 testbuddyai
```
Replace `/path/to/your/repo` with the absolute path to your code repository.

3. Access the App
Frontend: Open http://localhost:3000 in your browser.

Backend API: Access http://localhost:8000/docs for the interactive API docs.

## Usage
1. Configure Your Repository
On the frontend, specify the repository path (mounted via Docker) or let TestBuddyAI auto-detect it.

2. Run Tests
The AI will analyze your code, generate tests, and execute them automatically.

Check the dashboard for test coverage, results, and issue reports.

3. Review Suggestions
View detailed reports and apply suggested fixes to improve your codebase.

Example
For a Python file math_utils.py:
```python

def add(a, b):
    return a + b
```
TestBuddyAI generates:
```python

def test_add():
    assert add(2, 3) == 5
    assert add(-1, 1) == 0
```
Runs the tests and reports any failures.

## Project Structure

```
TestBuddyAI/
├── frontend/        # React frontend code
├── backend/         # FastAPI backend with AI logic
├── tests/           # Generated test files
├── Dockerfile       # Docker configuration
└── README.md        # This file
```

## Why TestBuddyAI?
Efficiency: Automates tedious test-writing tasks.

Intelligence: Leverages AI to create meaningful tests.

Privacy: Runs locally with no external dependencies.

Showcase: A great addition to your GitHub portfolio!

## Contributing
Feel free to fork this repository, submit issues, or create pull requests. Contributions are welcome!
Fork the repo.

Create a new branch (git checkout -b feature/your-feature).

Commit your changes (git commit -m "Add your feature").

Push to the branch (git push origin feature/your-feature).

Open a Pull Request.

## License
This project is licensed under the MIT License. See the LICENSE file for details.
## Contact
Built by [Wu Peng]. Reach out via [wupeng1127@gmail.com(mailto:wupeng1127@gmail.com)] or your GitHub profile.
Happy coding with your Test Buddy! 

