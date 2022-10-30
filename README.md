## Deploy grav to azure

- Connect webapp to github ![](.github/assets/2022-10-30-15-40-28.png)
- Add startup.sh in the settings ![](.github/assets/2022-10-30-15-44-39.png)

```bash
#!/bin/bash
cp /home/site/default.conf /etc/nginx/sites-available/default
service nginx reload
```

- Add default.conf file to `/home/site` (view sample in this repo)
- Install https://github.com/trilbymedia/grav-plugin-git-sync plugin on grav
- Configure git repository setting with your repo ![](.github/assets/2022-10-30-16-07-30.png)
