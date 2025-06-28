# Green Contribution Calendar 🟩

This project uses a GitHub Actions workflow to automatically commit to this repository every day, helping to keep your GitHub contribution calendar looking green.

## Setup

1. Fork this repository.
2. Enable Github Action.
3. Open the `.github/workflows/auto-commit.yml` file.
4. Find the following lines and **replace the placeholder values** with your actual GitHub username and email. 
    ```yaml
    git config --global user.name "Your Name"
    git config --global user.email "your-email@example.com"
    ```

5. Save the changes.
6. Leave fork network:

   Go to the repository’s Settings, scroll down to the `Danger Zone`, and click `Leave fork network.`

That's it! The workflow will now run automatically at the scheduled time. You can check the "Actions" tab in your GitHub repository to see the workflow runs.
