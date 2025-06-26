# Green Contribution Calendar 🟩

This project uses a GitHub Actions workflow to automatically commit to this repository every day, helping to keep your GitHub contribution calendar looking green.

## How It Works

The workflow is defined in `.github/workflows/auto-commit.yml`. It runs on a daily schedule (CRON job).

Here's what the script does:
1.  Checks out the repository.
2.  Configures Git with your username and email.
3.  Appends the current date and a message to a file named `daily-log.txt`. This ensures there is a file change to commit.
4.  Commits the change with a standardized message.
5.  Pushes the commit to the `main` branch.

## Setup

1.  **Clone this repository** to your local machine.
2.  **IMPORTANT**: Open the `.github/workflows/auto-commit.yml` file.
3.  Find the following lines and **replace the placeholder values** with your actual GitHub username and email. This is crucial for the contributions to be linked to your account.

    ```yaml
    # 1. Set up Git
    git config --global user.name "Your Name"
    git config --global user.email "your-email@example.com"
    ```

4.  Commit and push the changes:
    ```bash
    git add .
    git commit -m "feat: Initial commit with setup"
    git push origin main
    ```

That's it! The workflow will now run automatically at the scheduled time. You can check the "Actions" tab in your GitHub repository to see the workflow runs.
