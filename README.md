# Arch-Package-list
Simble bash script to push list of all packges installed on Your Arch Linux to the GitHub repo.
Perfect to be put in ```/etc/cron.daily/```  catalog.
## Instalation
Change 3rd line of script so it points to your repo: ```git clone https://github.com/YOUR-USER-NAME/YOUR-REPO-NAME.git```</br>
Put file in ```/etc/cron.daily``` for daily update or in ```/etc/cron.weekly``` for weekly update</br>
```sudo chmod +x /etc/cron.daily/push-new-package-list``` on the script to make it executable</br>
Make sure that cron daemon is running ```systemctl enable cronie``` (cronie is example cron implementation yours could be different)

## TODO
Script may be improved by checking if list of packages changed since last report, ergo not pushing the new list
