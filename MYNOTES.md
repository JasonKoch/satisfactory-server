Source releases: https://github.com/wolveix/satisfactory-server/releases

`git remote add upstream https://github.com/wolveix/satisfactory-server`

To update (not tested after fork and upstream version 1.8.7):
- Termanal open to D:\satisfactory-server
- `docker compose stop`
- `git fetch --tags upstream`
- `git rebase upstream/main` or `git rebase tags/x.x.x`
- `docker compose -f .\docker-compose.yml -f .\docker-compose.override.yml up -d --build`