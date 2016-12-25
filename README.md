# **BetterShutdown Reloaded**
BetterShutdown is a plugin that makes your server restarts and stops look better for your players.
It kicks all players to a predefined list of lobbies randomly, with a customizable message sent to them.

## Roadmap
I'm planning to add a lot new features to this project, and you can suggest more if you want to by clicking here.
- [x] Remaking the plugin based on the old code
- [x] Adding the ability to change the amount of time the server has to kick everyone out
- [ ] Add an auto updater so you won't have to worry of being up to date
- [ ] Adding variables on leave and stop messages
- [ ] Add the posibility to set specific servers for sepecific ranks

**NOTE:** *All plans mentioned here can change in order, can change the way they work or they can even be removed from the roadmap.*

## Configuration file
The plugin offers some customization via the config file. That includes the ability to change the messages sent when someone joins and the server is kicking everyone out to the lobbies, the message sent to the players when they are sent to the lobby. And the ability to change the amount of time the server has to kick all online players, which is very useful for servers with a high amount of players.
```yaml
# In here, you'll need to place a list of servers the players will be kicked to
# The name of them should be the same as their names on your BungeeCord config
# You can place as many as you want, but make sure they all exist on your BC config
Servers:
 - lobby1
 - lobby2


# This is the message the player will see when they get sent to another server
# You can use color codes on this setting
LeaveMessage: '&cYou have been moved to a lobby server.'

# This is the message a player will see when they try to join while the server is stopping
# You can use color codes on this setting
StopMessage: '&cThis server is safely stopping. Please wait a few seconds for it to come back online.'

# This number is the amount of seconds the plugin uses to kick all players before stopping the server
# In some servers, the default option (5) may not be enough due to a large amount of players connected
# If you are experiencing problems with certain players that are not moved to a lobby before stopping
# Increase this number to a higher value, but remember not to put ridiculously high numbers.
WaitTime: 5
```
