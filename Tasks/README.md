# Quantum AI Labs. Contribution and Submission Guide

This repository is used for educational tasks and grading.
All participants must follow the workflow below.
Failure to follow these rules may result in the submission not being graded.

---

## Overview

- This is a public repository
- Participants must fork the repository
- Participants must not push directly to the original repository
- All work is submitted via Pull Requests
- The main branch of the original repository is protected
- There is a fixed submission deadline of one week

This workflow mirrors real open source contribution practices.

---

## Submission Deadline

- The deadline is exactly one week from the official start date
- Only commits pushed before the deadline will be considered
- Any commits after the deadline will be ignored
- Pull Requests do not need to be merged

Late submissions will not be graded.

---

## Step 1. Fork the Repository

1. Click the Fork button at the top right of this repository
2. This creates a personal copy under your GitHub account
3. All your work will happen inside your fork

Do not clone the original repository directly.

---

## Step 2. Clone Your Fork

Clone your fork to your local machine.

    git clone https://github.com/YOUR_USERNAME/Quantum_AI_Labs_QML.git
    cd Quantum_AI_Labs_QML

Verify your remote.

    git remote -v

You should see only origin at this point.

---

## Step 3. Add the Original Repo as Upstream

This step is required to receive future updates.

    git remote add upstream https://github.com/QuantumAI-lab/Quantum_AI_Labs_QML.git
    git remote -v

You should now see.

- origin → your fork
- upstream → original repository

This step is done once only.

---

## Step 4. Create Your Working Branch

Do not work directly on main.

Create a branch using your name or assigned ID.

Examples.
- qml-task-abdo
- student-07-qml
- submission-ahmed

    git checkout -b YOUR_BRANCH_NAME

All commits must be on this branch.

---

## Step 5. Complete the Tasks

- Follow the task instructions exactly
- Modify only the files related to your tasks
- Do not restructure the repository unless explicitly instructed

Commit regularly with clear messages.

    git add .
    git commit -m "Complete Task 1. data preprocessing"
    git push origin YOUR_BRANCH_NAME

---

## Step 6. Keep Your Fork Updated

The original repository may receive updates during the week.

### Option A. GitHub Web Interface

1. Go to your fork on GitHub
2. Click Sync fork
3. Click Update branch

This works if there are no conflicts.

---

### Option B. Command Line Method

    git checkout main
    git fetch upstream
    git merge upstream/main
    git push origin main

After updating main, merge it into your working branch if needed.

---

## Step 7. Open a Pull Request

1. Go to your fork on GitHub
2. Click Compare and Pull Request
3. Target branch must be main of the original repository
4. Title format example.

    [QML Submission] Abdo. Task 1 and Task 2

Only one Pull Request per participant is allowed.

Do not merge the Pull Request.
Instructors will review and grade it after the deadline.

---

## Important Rules

- Do not push to the original repository
- Do not work directly on main
- Do not merge your own Pull Request
- Do not change the repository structure
- Do not submit after the deadline

---

## How Grading Works

Grading is based on.

- Code correctness
- Code quality
- Commit history
- Clarity of implementation
- Completion of required tasks

Only the state of the Pull Request at the deadline will be graded.

---

## Common Mistakes to Avoid

- Working on main
- Forgetting to sync fork
- Opening multiple Pull Requests
- Pushing after the deadline
- Copying other participants solutions

---

## Final Notes

This workflow is intentional.
It reflects real world open source contribution and review processes.

If you follow these steps exactly, there will be no issues with submission or grading.
