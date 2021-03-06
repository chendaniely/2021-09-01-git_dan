# 2021-09-01: NYR Git Workshop

- `git init`: initialize git repository in current location
    - `pwd`: tell you where you are
- `git status`: tells you the git status
- `git add <FILE>`: addes <FILE> to the staging area
- `git commit`: opens text editor to commit things in staging
    - `git commit -m "TEXT"`: writes "TEXT" for the commit message

- `git log`: shows you the log
    - `git log --oneline`: shows you the oneline log
- `git diff`: diff current changes to last git state
    - `git diff <HASH>/HEAD~<NUM>`: diff current state to another commit

- `git checkout <HASH> <FILE>`: revert <FILE> to the version in <HASH>
- `git checkout <HASH>`: revert everything to <HASH> in a detached HEAD state
    - `git checkout main` / `git switch main`: to go back

## Remotes

- `git remote add <NAME> <URL>`: add a remote <NAME> using the <URL>
    - `git remote add origin XXXXX`

- `git remote -v`: shows you what remotes you have
- `git push <REMOTE> <BRANCH>`: push our local changes in <BRANCH> to <REMOTE>
- `git pull <REMOTE> <BRANCH>`: pull changes from <REMOTE> down to local computer <BRANCH>
- Conflicts may happen during push/pull sync

## Branches

- `git branch <NAME>`: create a branch where you are (i.e., HEAD)
- `git branch -a`: list all your branches
- `git switch <BRANCH>`: move HEAD to <BRANCH>
    - `git checkout <BRANCH>`: the "older" way to move to another branch

- `git switch -c <BRANCH>`: create and move to <branch> in 1 step
    - `git checkout -b <BRANCH>`: the "older" way to create and move to branch

- pull request: merging a branch on the remote (i.g., GitHub)
    - update PR by pushing to the branch
    - merge the PR in the remote
    - delete branch on remote
- `git fetch --prune`: delete any local references where the remote branch was deleted
- `git branch -d <BRANCH>`: delete <branch>
    - `git branch -D <BRANCH>`: force delte branch without merging

- quick link for example workflow: https://bi-sdal.github.io/training/help-faq.html

- `git rebase main`: rebases current branch against main

- use branch protection rules to force PRs and code reviews
    - include admins if you want it to apply to yourself

### Git Flow

- convention for naming branches
- main is the "production"
- dev is the development

