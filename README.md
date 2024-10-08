# Project Title: GitHub Collaboration Demo

## Overview
This project is designed for hands-on practice in Git and GitHub collaboration. It demonstrates typical workflows used in team projects, including branching, making changes, creating pull requests (PRs), managing issues, and merging changes.

## Features
- Git commands for local and remote collaboration
- Branching for new features or bug fixes
- Creating and linking issues with PRs
- Code review and merging PRs
- Best practices for naming conventions and commit messages

## Getting Started

### Prerequisites
- A GitHub account
- Git installed on your local machine
- Basic understanding of Git and GitHub workflows

### Setup Instructions

1. **Fork the Repository**
   Before cloning the repository, you must first fork it to your GitHub account. This creates a copy of the repository under your own GitHub profile:
   - Navigate to the [GitHub Repository](https://github.com/SRM-IST-KTR/git-demo).
   - Click the **Fork** button at the top-right corner of the repository page.
   - Now, you will have a forked version of the repository under your GitHub account.

2. **Clone the Forked Repository**
   After forking the repository, clone your forked version to your local machine using the following command:
   ```bash
   git clone https://github.com/YOUR-USERNAME/git-demo.git
   ```
   Replace `YOUR-USERNAME` with your GitHub username. This will download your forked repository locally so you can work on it.

3. **Make Changes**
   Open any file (e.g., `README.md`) and make some edits. For example, you could add your name to the **Contributors** section or modify the content slightly to demonstrate collaboration.

4. **Create a New Branch and Switch to It**
   Create a new branch for your changes and switch to it:
   ```bash
   git checkout -b bugfix/typo
   ```
   **Branch Naming Conventions:**
   - Use descriptive branch names based on the task.
     - `feature/` for new features
     - `bugfix/` for fixing bugs
     - `hotfix/` for urgent changes
   - Use hyphens `-` to separate words in branch names.
   - Example: `feature/update-readme`, `bugfix/fix-typo`, `hotfix/security-patch`

5. **Add Files**
   Stage your changes by adding the modified files:
   ```bash
   git add .
   ```
   This prepares the files for committing.

6. **Commit Files**
   Commit your changes with a meaningful commit message:
   ```bash
   git commit -m "Add contributor name to README"
   ```
   **Commit Message Best Practices:**
   - Use the imperative mood: "Add feature" instead of "Added feature".
   - Keep the message concise but descriptive.
   - If necessary, include additional details in the body of the commit message by adding a blank line after the title and writing a more detailed explanation.

   Example:
   ```
   Fix typo in project overview

   Corrected a small typo in the first paragraph of the README file. 
   This improves clarity for readers.
   ```

7. **Push Files**
   Push your branch to GitHub:
   ```bash
   git push --set-upstream origin branch-name
   ```
   This will push your local branch to your forked repository on GitHub.

8. **Create an Issue**
   Before creating a PR, create an issue that describes the changes or feature you are adding. This helps track contributions and tasks:
   - Go to the **Issues** tab in your forked repository on GitHub.
   - Click on **New Issue**, fill in the details, and submit it.

   **Issue Best Practices:**
   - Write a clear, concise title (e.g., "Add contributor section to README").
   - Provide context and details about the task in the description.

9. **Create a Pull Request (PR)**
   After pushing the changes, open a pull request from your forked repository to the original repository:
   - Navigate to the original repository on GitHub.
   - Click on the **Compare & pull request** button.
   - In the PR description, link the issue by using `Closes #issue-number` (e.g., `Closes #1`).

   **PR Best Practices:**
   - Use a clear, action-oriented title: "Update README to include contributor info".
   - Provide a detailed description of what changes were made.
   - Reference the issue number so the PR is linked to the issue.

10. **Add Labels and Info to PR**
    Add relevant labels to the PR to help with project management:
    - Labels such as `enhancement`, `bug`, `documentation`, etc., can be applied.
    - You can also request a reviewer if you're working on a collaborative project.

11. **Merge the Pull Request (PR)**
    After your changes are reviewed and approved, merge the pull request:
    - Go to the PR on GitHub and click on **Merge Pull Request**.
    - When merging, mention the related issue (e.g., `Closes #1`), so the issue is automatically closed after merging.

## Contributing Guidelines

1. **Branch Naming Conventions**
   - Always create a new branch for each task:
     - `feature/` for new features (e.g., `feature/add-new-section`)
     - `bugfix/` for bug fixes (e.g., `bugfix/fix-footer-bug`)
     - `hotfix/` for urgent fixes (e.g., `hotfix/critical-security-fix`)
   - Be descriptive and consistent in your branch names.

2. **Commit Message Guidelines**
   - Write concise and meaningful commit messages.
   - Use the imperative mood in commit titles.
   - Optionally, add additional details in the body of the commit for clarity.

3. **Opening Issues**
   - Always create an issue for new features or bugs.
   - Write clear issue titles and descriptions, and assign relevant labels.

4. **Creating Pull Requests**
   - Reference the issue you are addressing in the pull request description.
   - Add labels and request reviews when necessary.

5. **Merging Pull Requests**
   - Before merging, ensure all comments and feedback are addressed.
   - Mention the related issue in the merge commit to close the issue automatically.