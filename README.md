# CI Lint + Test Pipeline


This project demonstrates a CI pipeline with:

- Code Linting (flake8)
- Automated Testing (pytest)
- Pipeline Stages Concept
- Job Dependency using `needs`

---

## 🛠 Tech Stack

- Python 3.9
- pytest
- flake8
- GitHub Actions

---

## 🔄 Pipeline Workflow

The CI pipeline consists of two stages:

### 1️⃣ Lint Stage
- Checks Python code style using flake8
- Ensures code quality
- Fails pipeline if lint errors found

### 2️⃣ Test Stage
- Runs unit tests using pytest
- Executes only after successful lint stage
- Uses `needs: lint` for stage dependency

---

## 📂 Project Structure
ci-lint-test-pipeline/ 
├── app.py 
├── test_app.py 
├── requirements.txt 
├── Dockerfile 
└── .github/workflows/ci-lint-test.yml

---

## 🚀 How It Works

On every push to `main` branch:

1. Lint job runs
2. If successful → Test job runs
3. If both pass → Green pipeline

---

## 🎯 Learning Outcomes

- CI Stage Separation
- Quality Gates in Pipelines
- Job Dependencies
- Automated Testing in CI
- Code Linting Integration

---

## 🏁 Status

✔ Lint Stage  
✔ Test Stage  
✔ Multi-stage Pipeline  

