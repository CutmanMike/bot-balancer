# Bot Balancer
Bot Balancer is a mod that adds bots to Zandronum servers, then removes them as human players arrive.

The purpose of this mod is to give players something to do while waiting for human players to arrive in their server, removing the bots when they are no longer needed. It also has a second function, which tries to prevent bot only LMS matches from soft locking by teleporting bots near eachother when no human players remain.

## Server Config
### botbalancer_botcount
Defines how many bots (per team) to add to the game (Default is **3**).

### botbalancer_detectgame
Detects what sort of game you're playing and fills the bot name list with appropriate bots. If nothing special is detected they will be filled with basic colour coded marine bots. Currently GVH and Mega Man 8-bit Deathmatch can be detected. Disable this if you want to go through the effort of making your own bot name lists. (default is **true**).

### botbal_fastforwardlms
Enables LMS "fast forwarding" when only bot players remain in a round. Bots will be teleported near eachother to battle it out, instead of stalling or soft locking the game (default is **true**).

### botbalancer_team_X_botY
Define what bot you want to use for this slot. *X* is the team number (1-4) and *Y* is the bot number (1-12). In non team games, only team 1 is used. Be sure to disable **botbalancer_detectgame** if you wish to customize the bot list.

## Limitations
* Having multiple bots of the same name will cause problems. This is due to the limited RemoveBot command which only takes player names. To get around this just make mew bots in a BOTINFO with different names.
* You can only have a maximum of 4 teams and 12 bots per team currently.

## Download

https://allfearthesentinel.com/zandronum/download.php?file=botbalancer-1b.pk3
