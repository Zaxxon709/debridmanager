# Debrid Manager

### How the addon works:
- Once authorization is complete a check is done for each supported addon to confirm if the addon is installed and if settings.xml exsists for that addon.
- If both of these checks are true all debrid data is then retrieved from Debrid Manager and applied to all the supported addons.

### Note for builders:
- For Debrid Manager to function correctly you need to ensure the directories containing your installed addons settings.xml are present in the addon_data directory.
- The reason for this is that some addons do not create the settings.xml after installation. The user first has to open the addons settings menu for it to be created. If it's not present Debrid Manager simply does nothing and moves on to the next addon.



### How to Authorize:

- Select Authorize and proceed to pair your account
- Wait for the 'Sync is complete' notification and choose OK to save 
- All supported add-ons included with the build are now authorized
- You can now exit and start streaming! 




### Authorize:
<ul>
Real-Debrid\
RunScript(script.module.myaccts, action=realdebridAuth)\
Premiumize\
RunScript(script.module.myaccts, action=premiumizeAuth)\
AllDebrid\
RunScript(script.module.myaccts, action=alldebridAuth)\
</ul>




### Sync Additional Addons:

Real-Debrid - RunScript(script.module.myaccts, action=realdebridSync)
Premiumize - RunScript(script.module.myaccts, action=premiumizeSync)
AllDebrid - RunScript(script.module.myaccts, action=alldebridSync)

Sync Addons:
If you decide to install additional supported add-ons you can sync them to your debrid account with one click!




### View/Manage Debrid Data:

Real-Debrid - ActivateWindow(10001,plugin://script.module.myauth/?mode=realdebrid,return)
Premiumize - ActivateWindow(10001,plugin://script.module.myauth/?mode=premiumize,return)
AllDebrid - ActivateWindow(10001,plugin://script.module.myauth/?mode=alldebrid,return)

View/Manage Debrid Data:
This feature allows the user to see what addons are currently authorized and provides a 1-click option to revoke all authorizations.