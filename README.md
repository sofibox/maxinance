# maxinance
Maxinance is a bash script that control web maintenance status via .htaccess. It can be used to put all website in directadmin into maintenance mode when doing a backup to prevent data integrity error. This maintenance operation is controlled by server.


Can put maintenance mode for specific webuser or website with single command:

This will put all website belongs to user abc into maintenance mode

`maxinance --set-offline --user abc`

This will put website web.com into maintenance mode

`maxinance --set-offline --user abc --website web.com`

It will also display a dynamic page maintenance mode that giving approximate time when it will finish.

It can automatically detect major websites to be put in maintenance mode via apache .htaccess

There will be a lot more feature such as putting directadmin system into maintenance mode (this feature is not available in directadmin itself but has been requested here: https://forum.directadmin.com/threads/maintenance-mode-for-updates-changes.59488/#post-318663 )
