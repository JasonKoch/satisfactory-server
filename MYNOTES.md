Source releases: https://github.com/wolveix/satisfactory-server/releases

<<<<<<< HEAD
`git remote add upstream https://github.com/wolveix/satisfactory-server`

To update (not tested after fork and upstream version 1.8.7):
- Termanal open to D:\satisfactory-server
- `docker compose stop`
- `git fetch --tags upstream`
- `git rebase upstream/main` or `git rebase tags/x.x.x`
- `docker compose -f .\docker-compose.yml -f .\docker-compose.override.yml up -d --build`
=======
To update (lightly tested as of 2024-09-21):
- Termanal open to D:\satisfactory-server
- `docker compose stop`
- `git fetch`
- `git rebase origin/main` or `git rebase tags/x.x.x`
- `docker compose build` (not 100% sure this will always rebuild)
- `docker compose up -d` (use the -d to detach from the started containers)
>>>>>>> caa3472 (add MYNOTES)
