#  User Manual Procedure

# Setting Up a GitHub Repository from Scratch and Making Your First Commit

## Before starting this procedure, ensure you have:

- A computer running Windows, macOS, or Linux with an active internet connection.
- A registered account on GitHub.com.
- Git installed on your computer. Verify this by running git --version in your terminal or command prompt.
- Basic familiarity with opening and typing commands in terminal/command prompt.

# Step-by-Step Procedure

## step 1:
- Open your web browser and log in to GitHub.
Navigate to [https://github.com](https://github.com) and sign in to your account.

- Expected Result: The main GitHub dashboard appears displaying your user feed and navigation header.

### step 2: 

- Open the repository creation form.

Click the + icon in the upper-right corner of any GitHub page and select New repository.

- Expected Result: The "Create a new repository" page opens.

### step 3:

- 
Configure your new repository details.

Type my-first-repo into the Repository name field, ensure Public is selected, and leave all checkboxes (Add a README file, Add .gitignore, Choose a license) unchecked.

- Expected Result: Green checkmark icon appears next to your repository name indicating it is available.

### step 4:

- Create the remote repository.

Scroll to the bottom of the page and click the green Create repository button.

- Expected Result: GitHub creates the empty repository and displays the "Quick setup" screen showing your repository's HTTPS URL (e.g., [https://github.com/your-username/my-first-repo.git](https://github.com/your-username/my-first-repo.git)).

### step 5:

- Open your local terminal or command prompt.

Windows: Press Win + R, type cmd, and press Enter.

macOS: Press Cmd + Space, type Terminal, and press Return.

- Expected Result: A terminal window opens displaying your user directory prompt.

### step 6:

- Create a local folder for your project and navigate into it.

Run:
mkdir my-first-repo && cd my-first-repo

- Expected Result: A new folder is created and your prompt updates to show my-first-repo as the current directory.

### step 7:

- Initialize local Git tracking in the folder.

Run:

git init

- Expected Result: Terminal displays Initialized empty Git repository in... and a hidden .git folder is created.

### step 8:

- Create a file to commit.

Run: 
echo "# My First Repository" > README.md
- Expected Result: A file named README.md containing the header text # My First Repository is saved in your directory.

### step 9:
- Stage the file for your commit.

Run:

git add README.md

- Expected Result: README.md is added to the Git staging area without error messages.

### step 10:

- Create your first commit locally.

Run:
git commit -m "Initial commit: Add README"

- Expected Result: Terminal outputs [main (root-commit) ...] (or [master ...]) showing 1 file changed and 1 insertion. 

### step 11:

- Set the default branch name to main.

Run: 
git branch -M main
- Expected Result: Local branch is renamed to main without throwing any errors.

### step 12:
- Connect your local Git repository to your GitHub repository.

- Replace YOUR-USERNAME with your actual GitHub username and run:

git remote add origin https://github.com/YOUR-USERNAME/my-first-repo.git

- Expected Result: The remote pointer named origin is attached silently.

### step 13:

- Push your local commit to GitHub.

Run:

git push -u origin main

- Expected Result: Terminal shows upload progress and concludes with Branch 'main' set up to track remote branch 'main' from 'origin'. Refreshing your repository page on GitHub now displays your README.md file online.

