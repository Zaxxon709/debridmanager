# Debrid Manager

### How the addon works:
- Once authorization is complete a check is done for each supported addon to confirm if the addon is installed and if settings.xml exists for that addon.
- If both of these checks are true debrid data is then retrieved from Debrid Manager and applied to the supported addon.

### Note for users/builders:
- For Debrid Manager to function correctly you need to ensure the directories containing the settings.xml for each supported addon are present in the addon_data directory.
- Some addons do not create the settings.xml after installation. To create it the user first has to open the addon settings menu and then choose 'ok' for the file to be created. If it's not present Debrid Manager simply does nothing and moves on to the next addon. So make sure to add these to your build.



### How to Authorize:
<ul>
    <li>Select Authorize and proceed to pair your account</li>
    <li>Wait for the 'Sync is complete' notification and choose OK to exit</li>
    <li>All supported add-ons included in your build are now authorized</li>
    <li>You can now exit and start streaming!</li><br>
</ul>



### Authorize:

<p>Real-Debrid<br>
RunScript(script.module.myaccts, action=realdebridAuth)</p>

<p>Premiumize<br>
RunScript(script.module.myaccts, action=premiumizeAuth)</p>

<p>AllDebrid<br>
RunScript(script.module.myaccts, action=alldebridAuth)</p><br>




### Sync Additional Addons:

<p>Real-Debrid<br>
RunScript(script.module.myaccts, action=realdebridSync)</p>

<p>Premiumize<br>
RunScript(script.module.myaccts, action=premiumizeSync)</p>

<p>AllDebrid<br>
RunScript(script.module.myaccts, action=alldebridSync)</p>


Sync Addons:
If you decide to install additional supported add-ons you can sync them to your debrid account with one click!<br><br>




### View/Manage Debrid Data:

<p>Real-Debrid<br>
ActivateWindow(10001,plugin://script.module.myauth/?mode=realdebrid,return)</p>

<p>Premiumize<br>
ActivateWindow(10001,plugin://script.module.myauth/?mode=premiumize,return)</p>

<p>AllDebrid<br>
ActivateWindow(10001,plugin://script.module.myauth/?mode=alldebrid,return)</p>


View/Manage Debrid Data:
This allows the user to see what addons are currently authorized and provides a 1-click option to revoke all authorizations.<br><br>



### Supported Addons:

1.  Seren<br>                   
2.  Ezra<br>                    
3.  Fen<br>                     
4.  Umbrella<br>             
5.  Shadow<br>               
6.  Ghost<br>                  
7.  Genocide<br>             
8.  Chain Reaction<br> 
9.  Twisted<br>
10. Base19<br>
11. Magic Dragon<br>
12. Asgard<br>
13. M.E.T.V<br>
14. Premiumizer<br>
15. My Accounts<br>
16. ResolveURL