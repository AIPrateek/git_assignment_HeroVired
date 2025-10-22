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

<br/>

<h1>Q3.<h1/>
Q.3: In this same GitHub repository, create a new branch ‘geometry-calculator’, we'll work on a simple Python program that calculates the area of a circle and the area of a rectangle. We'll use Git stash to switch between working on multiple features (calculating circle area and calculating rectangle area) without committing incomplete changes.

import math class GeometryCalculator: def calculate_circle_area(self, radius): return math.pi * radius ** 2

def calculate_rectangle_area(self, length, width): return length * width

if name == "main": calculator = GeometryCalculator()

TODO: Implement the feature to calculate the area of a circle radius = 5 print(f"The area of the circle with radius {radius} = {calculator.calculate_circle_area(radius)}")

TODO: Implement the feature to calculate the area of a rectangle # length = 10 width = 6 print(f"The area of the rectangle with length {length} and width {width} = {calculator.calculate_rectangle_area(length, width)}")

Workflow Steps: a. Create a New Branch:

Create a new branch named "feature/circle-area" to work on the circle area feature b. Stash Changes for Circle Area Feature:
Before committing the changes, stash them using git stash to save the incomplete feature implementation.
Verify that the working directory is clean c. Create a New Branch for Rectangle Area Feature:
Create a new branch named "feature/rectangle-area" to work on the rectangle area d. Stash Changes for Rectangle Area Feature:
Before committing the changes, stash them using git stash to save the incomplete feature implementation.
Verify that the working directory is clean e. Switch Back to Circle Area Branch:
Switch back to the "feature/circle-area" branch to continue working on the circle area feature.
Retrieve the stashed changes
Complete the circle area feature implementation and save the changes. f. Commit and Push Circle Area Feature: g. Switch Back to Rectangle Area Branch:
Switch back to the "feature/rectangle-area" branch to continue working on the rectangle area feature.
Retrieve the stashed changes
Complete the rectangle area feature implementation and save the changes. h. Commit and Push Rectangle Area Feature i. Create Pull Requests:
Create a pull request to the ‘dev’ branch. j. Review and Merge
Have another team member or reviewer review your pull requests. - After receiving approval, merge both pull requests into the main branch.
Answer
Step1: git checkout -b geometry-calculator
Step2: Made the required changes in the new python file geometry.py and saved it.
Step3: git add .
Step4: git commit -m "message"
Step5: git push -u origin geometry-calculator
Step6: git checkout -b feature/circle-area
Step7: Made the required change in the geometry file
Step8: git stash
Step9: git checkout geometry-calculator
Step10: git checkout -b feature/rectangle-area
Step11: Made the required change in the geometry file
Step12: git stash
Step13: git checout feature/circle-area
Step14: git stash list
Step15: git add .
Step16: git stash apply stash@{1}
Step17: git commit -m 'messsage'
Step18: git push -u origin feature/circle-area
Step19: Repeated the same steps from Step13 to Step18 for branch feature/rectangle-area
Step20: Requested two pull requests to merge both feature branches to dev, got it approved and merged.
Step21: Requested one pull request to merge dev to main, got it approved and merged.
