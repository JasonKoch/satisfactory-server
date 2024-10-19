Source releases: https://github.com/wolveix/satisfactory-server/releases

`git remote add upstream https://github.com/wolveix/satisfactory-server`

To update (tested once after fork and upstream version 1.8.7 --> 1.8.9):
- Termanal open to D:\satisfactory-server
- `docker compose stop`
- `git fetch --tags --force upstream`
- `git rebase tags/x.x.x or git rebase upstream/main`
- `git push`
- `docker compose -f .\docker-compose.yml -f .\docker-compose.override.yml up -d --build`
