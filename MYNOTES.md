Source releases: https://github.com/wolveix/satisfactory-server/releases

To update (lightly tested as of 2024-09-21):
- Termanal open to D:\satisfactory-server
- `docker compose stop`
- `git fetch`
- `git rebase origin/main` or `git rebase tags/x.x.x`
- `docker compose build` (not 100% sure this will always rebuild)
- `docker compose up -d` (use the -d to detach from the started containers)
