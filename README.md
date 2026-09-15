# SE-Git-hw

This repository contains my work for Assignment 1 in CINS 5318 Software Engineering.

## Purpose

This project demonstrates core Git and GitHub skills: creating a repository, branching, 
collaborating through pull requests, resolving merge conflicts, and tracking work with Issues.

## Programs

### Hello World

    python3 hello.py

**Expected output:**

    Hello, World! From main and conflict-demo, the conflict is now resolved!

### Apple Program

    python3 apple.py

**Expected output:**

    I eat apple

## Git and GitHub Workflow

1. Created the repository on GitHub and cloned it locally.
2. Added `hello.py` and committed it as the initial commit.
3. Created a `feature-1` branch, added `apple.py`, and pushed it to GitHub.
4. Opened a pull request to merge `feature-1` into `main`, had it reviewed, and merged it.
5. Used GitHub Issues to track and document remaining tasks.

## Merge Conflict Demonstration

Two branches, `main` and `conflict-demo`, both edited the same line in `hello.py` after 
diverging from a shared starting point. Attempting to merge `conflict-demo` into `main` 
caused Git to flag a content conflict on that line.

The conflict was resolved by opening the file, removing Git's conflict markers 
(`<<<<<<<`, `=======`, `>>>>>>>`), and manually combining both edits into a single line:

    print("Hello, World! From main and conflict-demo, the conflict is now resolved!")

The resolved file was staged, committed, and pushed back to `main`.
