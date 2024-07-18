
Objective:

- Familiarize with the basic workflow of creating a GitHub repository, connecting it to a local folder, and making commits and pushes.



Requirements:

- A GitHub account (create one if you don't have it already).

- A GitHub private access token (https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/managing-your-personal-access-tokens)

- Git installed on your local machine.

- A code editor of your choice (e.g., Visual Studio Code, Sublime Text).




Task 1: Repository Setup

1. GitHub Repository Creation:

  - Log in to your GitHub account.

  - Create a new repository on GitHub (let's call it "PLPBasicGitAssignment").

  - Initialize it with a README file.

  - Generate or use an exiting access token (refer to Requirements section to find more information about access tokens)



Task 2: Local Setup

2. Local Folder Setup:

  - Create a new folder on your local machine (e.g., "PLPBasicGitAssignment").

  - Open a terminal or command prompt and navigate to the created folder.

3. Git Initialization:

  - Initialize a new Git repository in your local folder.

4. Connecting to GitHub:

  - Link your local repository to the GitHub repository you created in Task 1.

   ```

   git remote add origin https://<access-token>@github.com/<username>/<repo>.git

   ```

   Replace <access-token>,<username>,<repo> with the actual details from your GitHub.



Task 3: Making Changes

5. Create a File:

  - Inside your local folder, create a new text file (e.g., `hello.txt`).

  - Add a simple text message (e.g., "Hello, Git!").


6. Update remote repository URLs

   ```bash

   git remote set-url origin https://<access-token>@github.com/<username>/<repo>.git


   ```

7. Committing Changes:

  - Stage the changes.

   ```bash

   git add hello.txt

   ```

  - Commit the changes.

   ```bash

   git commit -m "Add hello.txt with a greeting"

   ```



Task 4: Pushing to GitHub

7. Pushing to GitHub:

  - Push the committed changes to your GitHub repository.

   ```bash

   git push -u origin master

   ```


Task 5: Merging branches

8. Fetch the latest changes from the remote:

   ```bash

   git fetch origin

   ```

9. Check out the main branch:

   ```bash

   git checkout main

   ```

10. Rebase the main branch onto master:

   ```bash

   git rebase origin/master

   ```

11. Push the changes to the remote main branch:

   ```bash

   git push -f origin main

   ```
12. Push the changes to the remote main branch:

   ```bash

   git push origin --delete master

   ```


Task 6: Verification

13. Verify on GitHub:

  - Visit your GitHub repository in a web browser and confirm that the `hello.txt` file and commit message are visible.
