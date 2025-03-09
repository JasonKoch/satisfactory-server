Source releases: https://github.com/wolveix/satisfactory-server/releases

`git remote add upstream https://github.com/wolveix/satisfactory-server`

To update (tested once after fork and upstream version 1.8.7 --> 1.8.9):
- Termanal open to D:\satisfactory-server
- `docker compose stop`
- `git fetch --tags --force upstream`
- Pick your new target version and make a local branch to make the change: `git checkout -b rebase-x.x.x`
- `git rebase tags/x.x.x or git rebase upstream/main`
- `git push`
- `docker compose -f .\docker-compose.yml -f .\docker-compose.override.yml up -d --build`
- Merge the branch into main, then push: 
- `git checkout main`
- `git merge rebase-x.x.x`
- `git branch -d rebase-x.x.x`
- `git push`
