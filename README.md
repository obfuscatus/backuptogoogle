# backuptogoogle
---
# What script can do?
- Complie gdrive on your server with your Google credential
- Create cron auto backup
- Auto remove old backup on Google Drive
- Run upload from to Google Drive whenever you want
- Detail log
# OS support(x86_64):
- CentOS
- Debian
- Ubuntu
---
# How to use
Run command:
```
curl -o butgg.sh https://raw.githubusercontent.com/mbrother2/backuptogoogle/master/butgg.sh
sh butgg.sh --setup
```
# Options
Run command `sh butgg.sh --help` to show all options( After install you only need run `butgg.sh --help`)
```
Usage: butgg.sh [options] [command]

Options:
  --help      show this help message and exit
  --setup     setup or reset all scripts & config file
    no-build  setup or reset all scripts & config file without build gdrive
  --update    update to latest version
  --uninstall uninstall butgg.sh
```
# Command
###### 1. Help
```
butgg.sh --help
```
Show help message and exit
###### 2. Setup
```
butgg.sh --setup
```
Set up or reset all scripts & config file
```
butgg.sh --setup no-build
```
Setup or reset all scripts & config file without build gdrive
###### 3. Update
```
butgg.sh --update
```
Update to latest version
###### 4. Uninstall
```
butgg.sh --uninstall
```
Remove all butgg scripts and .gdrive directory
###### 5. Run upload to Google Drive immediately
```
cron_backup.sh
```
Run upload to Google Drive immediately without show log
```
cron_backup.sh -v
```
Run upload to Google Drive immediately with show log detail
