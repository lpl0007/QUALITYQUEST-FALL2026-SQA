
# Quality Quest - Fall 2026 SQA Project

## Team Members
- Lanie Louque
- Fabiya Mustari
- Nathan Evans

## Project Overview
Our team selected KubeSec, an existing Python-based project, to apply software quality assurance techniques.

The goal of this project is to practice software testing, identify potential issues, and improve software quality using different SQA activities.

## 1. Fuzz Testing
We used a Python fuzzing script (fuzz.py) to test the project with generated inputs.

Fuzz testing helps identify unexpected behavior, crashes, and potential software defects.

The fuzzing results are saved in fuzz-results.log during the GitHub Actions workflow.

## 2. Continuous Integration (CI)
We implemented continuous integration using GitHub Actions.

The workflow file is located at:
.github/workflows/sqa-ci.yml

Our workflow performs the following tasks:
- Checks out the repository.
- Sets up Python 3.11.
- Installs the required dependencies.
- Runs the fuzzing script.
- Saves the fuzzing output.
- Uploads the results as an artifact.

### CI Results
Our first workflow executions failed because of missing Python dependencies.

We reviewed the error messages and updated the dependency installation step.

After fixing the missing dependencies, the workflow ran successfully.

Successful workflow run: #4

Status: Success

Execution time: 21 seconds

Artifact generated: fuzzing-results

## 3. Software Forensics
This section will be updated after the team's software forensics analysis is completed.

## 4. Lessons Learned
Through this project, we learned how to:
- Configure a GitHub Actions workflow.
- Automate testing using continuous integration.
- Identify and fix missing dependency errors.
- Read GitHub Actions logs to troubleshoot failures.
- Save test results as workflow artifacts.
- Collaborate using a shared GitHub repository.

## Conclusion
Our team successfully configured a GitHub Actions workflow and executed automated fuzz testing.

This project helped us understand how continuous integration and software testing can support software quality assurance.
