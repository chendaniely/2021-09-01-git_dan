# NYR Git Workshop (2021-09-01)

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
    
