# Guideline how to implement solution for JS tasks
- Watch the videos in the topic Solving Tasks on GitHub:
  - in [English](https://mate.academy/en-gb/learn/javascript-advanced-en/solving-tasks-on-github-en?section=video)
  - in [Polish](https://mate.academy/pl/learn/javascript-advanced-pl/rozwiazywanie-zadan-github?section=video)
  - in [Ukrainian](https://mate.academy/learn/javascript-advanced/solving-tasks-on-github)
- Learn eslint rules from [the simplified styleguide](https://github.com/mate-academy/style-guides/blob/master/javascript.md)

## Prepare the project
1. Fork the repo (Github repository)
1. Clone the forked repo
    ```
    git clone the-link-from-your-forked-repo
    ```
    - You can get the link by clicking the `Clone or download` button in your repo
1. Open the project folder in your IDE
1. Open a terminal in the project folder
1. Create a branch for the solution and switch on it
    ```
    git checkout -b develop
    ```
    - You can use any other name instead of `develop`
1. Run `npm install` (or just `npm i`) to install the dependencies

## Implement the solution
1. Implement the solution within a function in `src/<task_name>.js`
    ![Where to write a solution](./assets/where-to-write-a-solution.png)
1. Run `npm run test` (or just `npm test`) to check if your solution is correct
    - If at least one test fails fix the solution and check again.
1. Run `npm run lint` to see if your code follows the [the simplified styleguide](https://mate-academy.github.io/style-guides/javascript-standard-modified)
    - If you see some errors fix them and check again
1. Save the solution
    ```
    git commit -am 'Solution'
    ```
    - code style is automatically checked again when you `commit` the code
    - Fix all the errors before committing again
1. Push the solution to the repo
    ```
    git push origin develop
    ```
    - If you created another branch (not `develop`) use its name instead
    - The tests are run again before the push to ensure the solution still works
    - Fix all the test and commit before pushing again
    
## Create a Pull Request (PR)
1. Open your repo on Github and create a `Pull Request` (PR)
    ![New PR button](./assets/new-pull-request-button.png)
1. Select your branch in the dropdown
    ![Create PR button](./assets/create-pull-request-button.png)
1. Verify the PR details and code (scroll down to see it) and confirm
    ![Create PR confirmation](./assets/create-pull-request-confirmation.png)

## If a mentor requested changes on your PR
1. Repeat [Implement the solution](#implement-the-solution) section
1. PR is updated automatically after a push to your branch on Github

> After updating your PR - click on re-request button at PR page IF YOU NEED ADDITIONAL REVIEW OF YOUR CODE.
![Image of re-request button](https://user-images.githubusercontent.com/38065883/104471439-89929200-55c3-11eb-824a-596bfb8aa246.png)
