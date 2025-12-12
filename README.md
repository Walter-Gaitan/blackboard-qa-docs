# Publishing Your Documentation

This folder (`public_docs`) contains **only** your documentation files. It is safe to publish this to a public GitHub repository to get free hosting.

## Steps to Publish

1.  **Create a New Repository on GitHub**
    *   Go to [github.com/new](https://github.com/new).
    *   Name it something like `blackboard-qa-docs`.
    *   Make sure it is **Public**.
    *   **Do not** initialize with specialized files (README, license, etc.), just create it empty.

2.  **Initialize this Folder**
    Open your terminal in this `public_docs` folder and run:
    ```bash
    git init
    git add .
    git commit -m "Initial commit of documentation"
    git branch -M main
    git remote add origin https://github.com/<YOUR_USERNAME>/blackboard-qa-docs.git
    git push -u origin main
    ```

3.  **Setup Complete!**
    *   The `GitHub Actions` workflow included here will automatically run.
    *   Wait for the action to finish (check the "Actions" tab on your new repo).
    *   Go to **Settings > Pages** in your new repo and ensure it's deploying from the `gh-pages` branch.
    *   Your site will be live at `https://<YOUR_USERNAME>.github.io/blackboard-qa-docs/`.
