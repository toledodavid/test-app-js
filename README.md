# Test App to practice git commands and integrations

First for all, begin defining names for working branches and commit names to have a standar in your repository.

For this repositoty we are going to follow the next standar names:

* If I want to add a new feature to the project then I am going to use this name to create the branch `review/ticket-number`

* If I want to fix a bug then I am going to use this name to create the branch `fix/ticket-number`

* For the commit messages I am going to start with the ticket number and then the title of the ticket or the changes that I did. For instance `T01: hello word added in MainPage`


Now I can start working!

### SCENARY 1:
I want to start working in a new feature or bug:
  1. move to `dev` branch: `git checkout dev`
  2. create my branch and move to ti to start working in my changes: `git checkout -b review/ticket-number`
  3. use `git branch` command to be sure that you are in your new branch. And you can start working in your changes.
  4. Once you have modified the files for your changes and you want to save them, then you can create a commit:
      1. `git add .`
      2. `git commit -m "ticket-number: message for the changes"`
  5. push your changes to GitHub for review:
      1. `git push origin review/ticket-number` this command is going to push your branch to GitHub.
      2. In GitHub you are going to be able to see an alert message to create a Pull request for your changes. Click the button `Create pull request` and verify the commit message, add the reviwers and create the pull request for review.
  6. Once your team have reviewed your PR and is approved then you can merge it and delete your branch.


### SCENARY 2:
I want to work in some changes for my PR because I missed something or my teammates suggested a change.