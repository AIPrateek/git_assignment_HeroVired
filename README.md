# git_assignment_HeroVired

Q.1: You are part of a development team working on a Python application called "CalculatorPlus." The application provides basic arithmetic operations, such as addition, subtraction, multiplication, and division. Your task is to implement a new feature that adds support for calculating the square root of a number. a. Create a repository name: git_assignment_HeroVired b. Create a ‘dev’ branch and add this code.

import math class Calculator: def add(self, a, b): return a + b def subtract(self, a, b): return a - b def multiply(self, a, b): return a * b def divide(self, a, b): return a / b

TODO: Implement the following function to calculate the square root of a number. def square_root(self, x): return math.sqrt(x) You need to uncomment the above function and complete its implementation to add the square root feature.

if name == "main": calculator = Calculator() num1 = 16 num2 = 4 print(f"{num1} + {num2} = {calculator.add(num1, num2)}") print(f"{num1} - {num2} = {calculator.subtract(num1, num2)}") print(f"{num1} * {num2} = {calculator.multiply(num1, num2)}") print(f"{num1} / {num2} = {calculator.divide(num1, num2)}")

TODO: Uncomment and test the square root feature. num3 = 25 print(f"The square root of {num3} = {calculator.square_root(num3)}")

c. Merge this branch with the main branch and make a release of version 1 of the ‘calculator plus app’. d. Add any of your classmates as collaborators. e. Implement a feature by creating a new branch called ‘feature/sqrt’. f. Add the ‘sqrt’ code to it. g. While you are working on this feature, imagine that one critical bug is reported in the main branch, and you need to switch back to the ‘dev’ branch, create fixes, and apply them while keeping your ‘feature/sqrt’ branch up-to-date. For this, you need to create

The bug fixation is in the divide function and the new function should be: def divide(self, a, b): if b == 0: raise ValueError("Cannot divide by zero.") return a / b

h. After completing the feature implementation and ensuring that the application works correctly, create a pull request targeting the main branch. i. Request a code review from a team member and make any necessary improvements based on the review feedback. j. Once the code reviewer approves your pull request, merge the "feature/sqrt" branch into the ‘dev’ branch. k. Finally, do the testing in the ‘dev’ branch itself and merge it into the ‘main’ branch and create a ‘version 2’ release.

Answer
Step1: Created a private repository in github
Step2: Cloned the repo in my system using the command 'git clone URL'
Step3: Created dev branch using the command 'git checkout -b dev'
Step4: Created a file calculator.py in the repo and updated the code mentioned in the question. Only addition, subtraction, divide and multiple functions to be working in dev branch.
Step5: Checked the status using the command 'git status'
Step6: Staged the changes using the command 'git add .'
Step7: Committed the changes using the command 'git commit -m 'message'
Step8: Pushed the changes to remote using the command 'git push -u origin dev'
Step9: Checkout to main branch to merge the changes made in dev to main branch (command used: git checkout main, git merge dev)
Step10: Created a new branch with feature/sqrt name (git checkout -b feature/sqrt)
Step11: Made the changes related to the square root function in the branch and then repeated the steps from Step5 to Step8 for the branch feature/sqrt.
Step12: Checkout to dev branch and fix the bug in the same branch ( commands used: git checkout dev)
Step13: Made the changes related to the bug in the dev branch and then repeated the steps from Step5 to Step8 for the branch dev.
Step14: Added my friend as a collaborator for the repo.
Step15: Raised a pull request from feature branch to dev branch. got it approved and merged both the branches.
Step16: Raised a pull request from dev branch to main branch. got it approved and merged both the branches.

