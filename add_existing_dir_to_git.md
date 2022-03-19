## This doc shows the steps through which you can start using git on some existing projects

### Here "my_recognition_cpp" is my working directory in which git has to be initialized and same has to be pushed to the main branch

1. `cd my_recognition_cpp`
2. `git init`
3. `git add .`
4. `git commit`
5. `git remote add my_recognition_cpp https://github.com/muditsingal/my_recognition_cpp.git`
6. `git push --set-upstream  my_recognition_cpp master`
7. `git checkout main`
8. `git merge master` please note that you will probably get the error **fatal: refusing to merge unrelated histories**
9. To resolve this just use the command- `git merge master --allow-unrelated-histories`
10. Now you can continue working on your project in the main branch with the added benifits of version control provided by git!
