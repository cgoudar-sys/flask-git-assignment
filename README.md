# Flask Git Versioning Assignment

This project is a small Flask web application created for practicing REST API endpoints and Git versioning. It starts with two basic endpoints and then adds a simple in-memory voting feature. The project follows a `dev` to `main` workflow so stable code is merged into `main` only after testing.

## Installation and Setup

Clone the repository:

```bash
git clone https://github.com/cgoudar-sys/flask-git-assignment.git
cd flask-git-assignment
```

Create and activate a virtual environment:

```bash
python3 -m venv venv
source venv/bin/activate
```

Install dependencies:

```bash
pip install -r requirements.txt
```

Run the application:

```bash
python app.py
```

Open the application in a browser:

```text
http://localhost:5000/
http://localhost:5000/health
http://localhost:5000/vote/Alice
http://localhost:5000/results
http://localhost:5000/reset
```

## API Endpoint Reference

| Endpoint | Method | Description | Example Response |
|---|---|---|---|
| `/` | GET | Displays the home page message. | `Welcome to the App` |
| `/health` | GET | Confirms that the app is running. | `App is running` |
| `/vote/<name>` | GET | Records one vote for the candidate name in the URL. | `{"candidate":"Alice","message":"Vote recorded for Alice","votes":1}` |
| `/results` | GET | Returns the current vote count for all candidates. | `{"Alice":1,"Bob":1}` |
| `/reset` | GET | Clears all stored vote counts. | `{"message":"All votes have been reset"}` |

## Git Workflow

Development work is completed on the `dev` branch. After each version is tested, `dev` is merged into `main`. This keeps `main` as the stable branch while still showing the full feature development history.

```text
dev  -> build and test feature
main <- merge completed version from dev
```

## Version History

| Version | Description |
|---|---|
| Version 1 | Added the basic Flask application with `/` and `/health` endpoints. |
| Version 2 | Added voting endpoints `/vote/<name>`, `/results`, and `/reset`. |

## Screenshots

Add your screenshots below before final submission:

1. Application running in browser.
2. GitHub repository showing both `dev` and `main` branches.
3. Commit or merge history showing Version 1 and Version 2 releases.
