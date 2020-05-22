# Participation

## Spotted an error?

Have you found any errors somewhere in the text? Would you like to contribute some challenges, cool URLs, or other CS facts?

## How can I contribute?

The way (some) software professionals do. Via pull requests on github. This booklet is shared [here](https://github.com/lancsunise/stayathome).

When developers work on a big project they use a version control system (e.g. git). Keeping code under a version control helps immensely to build software. But, a version control is not only limited to the code. Text, books, or virtually any files are allowed under a version control system, allowing you to see the whole history of files. The benefit of a version control system in our case is that if you find an error in the text, then you have the complete freedom to directly patch the error and create a pull request. If your correction is valid, I will merge the changes into the master branch.

## Branches and Pull Requests

The copy of this booklet lives on the master branch. To make changes, you need:

1. Clone the repository locally on your computer:
```
git clone https://github.com/lancsunise/stayathome
```
2. Create a new branch where you will apply a fix (you can replace my_fix_branch with any other name describing what you are fixing):
```
git checkout -b my_fix_branch
```
3. Before you apply the fix, you can check that the new branch has been created and you are on it (you're on the branch where git shows a star sign next to it (*)):
```
git branch
```
4. Apply the fix
5. Ideally, you use Linux and have the `pandoc` and `latex` software installed. If you do, you should run the `build.sh` script:
```
./path/to/the/script/stayathome/build.sh
```
6. Once you're happy with the changes, stage the file you just updated:
```
git add stayathome.md
```
7. Use git status to check that the file is staged:
```
git status
```
8. Now commit with a descriptive message:
```
git commit -m "fixing how to contribute description"
```
9. Now push your new branch upstream (to github):
```
git push -u origin my_fix_branch
```
10. Go to the repository from your browser:
```
https://github.com/lancsunise/stayathome/pulls
```
11. You should now see something like "Your recently pushed branches (x minutes ago)". Click on "Compare & pull request"
12. A new screen "Open a pull request" opens. Add any comments and finish by clicking on "Create pull request"
13. If you realised that you should change something more as part of this pull request, don't worry. Just stay on the same branch and add those changes.
14. Now repeat steps from 6 to 9. The new commit will be automatically added as part of the already opened pull request.
15. To finish, go back to the terminal and return to the master branch:
```
git checkout master
```
16. If you are sure you don't want to change anything else on your branch, you can delete it (only locally on your machine!):
```
git branch -d my_fix_branch
git branch
```
17. That's it. Once reviewed, your changes will be merged. Once enough changes are made, a new version may be released. 
