#  deploy script to /usr/local/bin
```bash
sudo cp auto_wallpaper/auto_wallpaper.sh /usr/local/bin
sudo chmod +x /usr/local/bin/auto_wallpaper.sh
```

# setting cron job
```bash
    crontab -e
```
add line
```
    -- run script every 1 minutes
    * * * * * /usr/local/bin/auto_wallpaper.sh

    -- run script every 3 minutes
    */3 * * * * /usr/local/bin/auto_wallpaper.sh
```