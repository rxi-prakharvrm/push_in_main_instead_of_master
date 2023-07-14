# Push in __main__ branch instead of __master__ branch

To update the remote origin URL for a GitHub repository, you can use the `git remote set-url` command. Follow these steps to update the remote origin URL:

1. Open Git Bash and navigate to your local repository's directory using the `cd` command:
```
cd /path/to/your/repository
```

2. Verify the current branch
```
git branch --show-current
```

3. Create a new main branch and switch on it
```
git switch -c main
```

4. Stage all the changes
```
git add .
```

5. Commit the changes
```
git commit -m "<commit msg>"
```

6. Add remote url
```
git add remote origin "<origin-url>"
```

7. Fetch
```
git fetch
```

8. Merge main branch to origin
```
git merge --allow-unrelated-histories origin/main
```

9. Push your code to the origin main
```
git push origin main
```
