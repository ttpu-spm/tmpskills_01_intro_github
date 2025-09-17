# Course Completion Tracking System

This repository includes an automated GitHub Actions workflow that allows students to submit their course completion information.

## How It Works

1. **Student Completes Course**: Student finishes the GitHub Skills Introduction course, which creates a repository in their personal GitHub account (e.g., `https://github.com/studentusername/introduction-to-github`)

2. **Student Submits Completion**: Student uses the GitHub Actions workflow to submit their completion:
   - Navigate to "Actions" tab in this repository
   - Select "Track Course Completion" workflow
   - Click "Run workflow" 
   - Enter their name and repository URL
   - Click "Run workflow"

3. **Automatic Processing**: The workflow:
   - Validates the repository URL format
   - Checks for duplicates
   - Adds the entry to README.md with timestamp
   - Commits and pushes the changes

## Workflow Features

- **URL Validation**: Ensures only valid GitHub repository URLs are accepted
- **Duplicate Prevention**: Prevents the same repository from being added multiple times
- **Automatic Formatting**: Adds entries in a consistent format with completion timestamp
- **Error Handling**: Provides clear error messages for invalid inputs

## Entry Format

Completed entries appear in the README as:
```
- **Student Name**: [https://github.com/student/introduction-to-github](https://github.com/student/introduction-to-github) (completed: YYYY-MM-DD)
```

## Maintenance

The system requires no maintenance. All processing is automated through GitHub Actions.