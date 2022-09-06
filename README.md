# example-changeset-update-of-dependant-modules
Example of changeset version updating dependant modules in a monorepo

## Run
To test this example run:
```
npm i
npx changeset version
```

And it should have modified all the package.json across that are dependant of the module `M`.
Running a git status show us the following:
```
git status
On branch main
Your branch is ahead of 'origin/main' by 2 commits.
  (use "git push" to publish your local commits)

Changes not staged for commit:
  (use "git add/rm <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        deleted:    .changeset/tasty-moons-double.md
        modified:   apps/X/package.json
        modified:   apps/Y/package.json
        modified:   libraries/M/package.json
        modified:   libraries/Z/package.json
...
```
