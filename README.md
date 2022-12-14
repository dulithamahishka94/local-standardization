# local-standardization
Githooks to standardize your local environment

## Prerequisites

 1. You need to have python installed.
 2. Currently this works only with Mac and Ubuntu. If you have a windows PC, you have to manually copy the contents inside .github/hooks to `<workspace>/.git/hooks` folder

## How does it work

 1. Clone this repository in your project root directory.
 2. Change the `project_code` in .`github/hooks/commit-msg` line 15 to your JIRA project ID. This will help to validate the commit messages against your project code.
 3. Execute below command from the root of your project directory (This will copy the GitHooks into .git folder). `./.github/hooks/update_hooks.sh`
 4. Please be noted that you will not be able to commit unless you follow the proper commit message validation standards given in the hook.
 5. Please be noted that you will be able to create branches with a name you desire in your local environment, but will not be able to push your branch into the remote unless you follow the proper branch naming standards given in the hook.
