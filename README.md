# CI GitHub Actions Demo

This repository demonstrates the use of GitHub Actions for Continuous Integration (CI) with Python.  
It includes several workflows that automate testing, scheduling, and multi-version builds.

---

#### **Task 1 – Basic GitHub Actions Workflow**

* Trigger: On every push to `main`
* Actions:
  * Checkout the code
  * Print a message: `Hello, CI with GitHub Actions!`
* Workflow file: `.github/workflows/basic-ci.yml`

---

#### **Task 2 – Running Tests**

* Added `main.py` and `test_main.py` for testing with `unittest`
* Workflow sets up Python 3.9, installs dependencies, and runs tests
* Workflow file: `.github/workflows/test-matrix.yml`

---

### **Part 2: Advanced GitHub Actions**

#### **Task 3 – Cron Scheduling**

* Runs automatically every day at midnight (UTC)
* Prints: `Scheduled build completed successfully!`
* Workflow file: `.github/workflows/scheduled-build.yml`

---

#### **Task 4 – Matrix Builds**

* Extended the test workflow to run on multiple Python versions:  
  `3.8`, `3.9`, `3.10`, and `3.11`
* Ensures compatibility across different environments

---

### **Set up Self Hosted Runner**

* Set up a **self-hosted runner** on a local machine or server.  
* Registered the runner in the repository settings under **Settings → Actions → Runners**.  
* Configured it to run one of the existing workflows instead of GitHub’s hosted runners.  
* Verified that the workflow successfully executed using the self-hosted runner.

