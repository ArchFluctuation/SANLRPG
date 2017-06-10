### SANLadmin
|Export|Sided|Parameters|Description|
|---|---|---|---|
|doesAccountHavePermission|Server|iAccount,strPermission|Checks whether iAccount has been assigned strPermission.|
|giveAccountPermission|Server|iAccount,strPermission|Assign strPermission to iAccount.|
|removeAccountPermission|Server|iAccount,strPermission|Remove assignment of strPermission to iAccount.|
|getAccountPermissions|Server|iAccount|Returns a table of every permission assigned to iAccount.|

### SANLcommands
|Export|Sided|Parameters|Description|
|---|---|---|---|
|sendMessage|Server|strMessage, playerElem, red, green, blue|Sends a message to the player's messagebox. Use 'false' for playerElem to send to all players.|
|sendClientMessage|Client|strMessage, red, green, blue [, funcFormattable]|Sends a message to the local player's messagebox. If you use %s in the strMessage, the return value of funcFormattable will show in real-time.|

### SANLcore
|Export|Sided|Parameters|Description|
|---|---|---|---|
|getAccountData|Server|accountID,strKey|Replacement for native MTA function (uses account ID, not username).|
|getPlayerAccount|Server|thePlayer|Returns the account ID of the player, if they're logged in (or false).|
|getPlayerUsername|Server|thePlayer|Returns the account username of the player, if they're logged in (or false).|
|setAccountData|Server|accountID,strKey,value|Replacement for native MTA function (uses account ID, not username).|

### SANLjobs
|Export|Sided|Parameters|Description|
|---|---|---|---|
|getPlayerCareerProgression|Server|thePlayer, strCareer|Returns the career progression (number) of thePlayer for strCareer.|
|getPlayerJob|Server|thePlayer|Returns the job name (string) of thePlayer.|
|getPlayersByJob|Server|strJob|Returns a table of all players currently employed as strJob.|
|getRankName|Server|strCareer, iProgression|Returns the rank name for strCareer at the level of iProgression.|
|getRankNumber|Server|strCareer, iProgression|Returns the rank number for strCareer at the level of iProgression.|
|isPlayerWorking|Server|thePlayer|Returns whether or not thePlayer is on-duty (boolean).|
|modifyPlayerCareerProgression|Server|thePlayer, strCareer, iProgression|Modify the career progression of thePlayer for strCareer by iProgresion.|
|removePlayerJob|Server|thePlayer|Forces thePlayer to resign from their job.|
|setPlayerCareerProgression|Server|thePlayer, strCareer, iProgression|Sets the career progression of thePlayer for strCareer to iProgression.|
|setPlayerJob|Server|thePlayer, strJob|Changes the job of thePlayer to strJob.|
|setPlayerWorking|Server|thePlayer, bWorking|Sets whether or not thePlayer is on-duty.|

### SANLsql
|Export|Sided|Parameters|Description|
|---|---|---|---|
|exec|Server|strQuery [, ...]|Executes an SQL query (without waiting for results).|
|query|Server|strQuery [, ...]|Executes an SQL query and polls results.|

### SANLtools
|Export|Sided|Parameters|Description|
|---|---|---|---|
|convertMoneyToString|Both|iMoney|Converts iMoney to to a nicely formatted string in U.S. Dollars with commas.|
|getElementSpeed|Client|theElement|Returns the movement speed (in KPH) of theElement.|
|getPlayerCountry|Server|thePlayer|Returns the name of the country the player is connected from, or "Unknown".|
|getPlayerRecord|Server||Returns the (numerical) record for most players online at once.|
