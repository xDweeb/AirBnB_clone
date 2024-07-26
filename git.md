To work with branches in GitHub, you can use Git commands from your command line interface (CLI). Here are the commands to see branches, create a new branch, and delete a branch:

### View Branches

To see the branches in your local repository, use:

```bash
git branch
```

To see all branches, including remote branches, use:

```bash
git branch -a
```

### Create a New Branch

To create a new branch and switch to it:

```bash
git checkout -b new-branch-name
```

Alternatively, you can create the branch without switching to it:

```bash
git branch new-branch-name
```

Then, switch to the new branch:

```bash
git checkout new-branch-name
```

To push the new branch to the remote repository (GitHub):

```bash
git push -u origin new-branch-name
```

### Delete a Branch

To delete a branch locally:

```bash
git branch -d branch-name
```

If the branch has not been merged and you want to force delete it:

```bash
git branch -D branch-name
```

To delete a branch on the remote repository:

```bash
git push origin --delete branch-name
```

### Example Workflow

1. **View branches:**

   ```bash
   git branch -a
   ```

2. **Create and switch to a new branch:**

   ```bash
   git checkout -b feature/new-feature
   ```

3. **Push the new branch to GitHub:**

   ```bash
   git push -u origin feature/new-feature
   ```

4. **Delete a branch locally:**

   ```bash
   git branch -d feature/old-feature
   ```

5. **Delete a branch on GitHub:**

   ```bash
   git push origin --delete feature/old-feature
   ```

These commands will help you manage branches in your Git repository both locally and on GitHub.