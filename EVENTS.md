### SANLcore
|Event|Sided|Source|Parameters|Description|
|---|---|---|---|---|
|onLogin|Server|thePlayer|accountID,accountUsername|Triggered when a player logs into their account.|
|onLogout|Server|thePlayer|accountID,accountUsername|Triggered when a player quits (since players cannot manually logout). This event is used to ensure account data is still available (i.e. the cache hasn't been cleared earlier in the frame).|
|onPlayerLifeBegin|Server|thePlayer||Triggered after a player selects their starting skin and has finished watching the introduction cinematic.|
|onPlayerChangeTeam|Server|thePlayer|theTeam|Triggered when a player is assigned to a different team.|


### SANLjobs
|Event|Sided|Source|Parameters|Description|
|---|---|---|---|---|
|onPlayerChangeJob|Server|thePlayer|newJob||
|onPlayerResign|Server|thePlayer|oldJob|Triggered when a player resigns or switches job.|
