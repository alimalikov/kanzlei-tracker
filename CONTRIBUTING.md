# Contributing to kanzlei-tracker

Thank you for contributing! This guide explains how to upload your local project folder to this repository.

---

## How to Upload Your Local Folder to This Repository

### Option 1: Using GitHub Desktop (Recommended for Beginners)

1. **Download GitHub Desktop** from <https://desktop.github.com/> and sign in with your GitHub account.
2. **Clone this repository**:
   - Open GitHub Desktop → **File → Clone repository**.
   - Search for `alimalikov/kanzlei-tracker` and click **Clone**.
   - Choose a local folder where the cloned repo will be saved (e.g., `C:\Projects\kanzlei-tracker`).
3. **Copy your files**:
   - Open your existing project folder in File Explorer / Finder.
   - Select all files and folders inside it and copy them.
   - Paste them into the folder where you cloned the repository (from step 2).
4. **Commit and push**:
   - Switch back to GitHub Desktop — it will show all new files as changes.
   - Fill in a **Summary** (e.g., `Add initial project code`).
   - Click **Commit to main**.
   - Click **Push origin** to upload the changes to GitHub.

---

### Option 2: Using Git on the Command Line

1. **Install Git** if you haven't already: <https://git-scm.com/downloads>

2. **Open a terminal** (Command Prompt, PowerShell, or Terminal on macOS/Linux).

3. **Clone this repository** into a temporary folder:
   ```bash
   git clone https://github.com/alimalikov/kanzlei-tracker.git
   cd kanzlei-tracker
   ```

4. **Copy your project files** into the cloned folder:
   ```bash
   # On Windows (PowerShell) — replace C:\path\to\your\folder with the actual path
   Copy-Item -Path "C:\path\to\your\folder\*" -Destination "." -Recurse

   # On macOS / Linux — replace /path/to/your/folder with the actual path
   cp -r /path/to/your/folder/. .
   ```

5. **Stage all new files**:
   ```bash
   git add .
   ```

6. **Commit the changes**:
   ```bash
   git commit -m "Add initial project code"
   ```

7. **Push to GitHub**:
   ```bash
   git push origin main
   ```

---

### Option 3: Using the GitHub Web Interface (Small Projects / Single Files)

This method works well if you only have a few files to upload.

1. Go to <https://github.com/alimalikov/kanzlei-tracker>.
2. Click **Add file → Upload files**.
3. Drag and drop your files (or click **choose your files** to browse).
4. Scroll down, add a short commit message, and click **Commit changes**.

> **Note:** The web interface does not support uploading entire folder structures easily. For larger projects, use Option 1 or Option 2 above.

---

## Branching Workflow

If you are making changes to an existing codebase (rather than an initial upload), please follow this workflow:

1. **Create a new branch** from `main`:
   ```bash
   git checkout -b feature/your-feature-name
   ```
2. **Make your changes**, commit them, and push the branch:
   ```bash
   git add .
   git commit -m "Describe your changes"
   git push origin feature/your-feature-name
   ```
3. **Open a Pull Request** on GitHub and request a review.

---

## Need Help?

If you run into any issues, open a [GitHub Issue](https://github.com/alimalikov/kanzlei-tracker/issues) and describe the problem.
