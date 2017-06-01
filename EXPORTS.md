### SANLcommands
|Export|Sided|Parameters|Description|
|---|---|---|---|
|sendMessage|Server|strMessage, playerElem, red, green, blue|Sends a message to the player's messagebox. Use 'false' for playerElem to send to all players.|
|sendClientMessage|Client|strMessage, red, green, blue [, funcFormattable]|Sends a message to the local player's messagebox. If you use %s in the strMessage, the return value of funcFormattable will show in real-time.|

### SANLjobs
|Export|Sided|Parameters|Description|
|---|---|---|---|
|getPlayerJob|Server|thePlayer|Returns the job name (string) of thePlayer.|
|getPlayersByJob|Server|strJob|Returns a table of all players currently employed as strJob.|
|isPlayerWorking|Server|thePlayer|Returns whether or not thePlayer is on-duty (boolean).|
|removePlayerJob|Server|thePlayer|Forces thePlayer to resign from their job.|
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
|getPlayerRecord|Server||Returns the (numerical) record for most players online at once.|
