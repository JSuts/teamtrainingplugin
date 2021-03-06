A Bakkesmod plugin for multiplayer custom training drills.

# Usage

For multiplayer training with non-local players, you can use [Rocket Plugin](https://bakkesplugins.com/plugins/view/26) for hosting a freeplay session that others may join.

Press F2, go to plugins, select Team Training Plugin, and click the button to launch the UI.

The new UI contains tabs for selecting training packs, assigning player roles, converting a custom training pack into a team training pack, and modifying the plugin's settings.

The plugin comes packaged with three packs: left, right, and infield. These packs were generated from Wayprotein's passing packs: C833-6A35-A46A-7191, 0590-9035-801A-E423, CDBB-8953-C052-654F. Note the shooter positions are a little awkward as they are positioned after the pass is in progress.

# Creating Team Training Packs

Team training packs can be created using regular custom training packs. The way this works is by setting each player's position in separate drills within the custom training pack, and the starting ball's state is taken from the first passer.

Entering the the number of offensive and defensive players in the Creation tab will show the drill order. For example, set offensive players to 3 and defensive players to 1. The drill order shows that the first drill should be the shooter's position, the second drill will be the second passer position (passes to shooter from first passer's pass), the third drill will be the first passer position AND the ball's starting position and trajectory in the team training drill, and the fourth drill will be the defender's position. These 4 drills will make up one team training drill. Repeat this pattern in the same custom training pack to have more than one team training drill.

Once you have prepared your custom training pack, open the custom training pack to the first drill, open the Team Training plugin's UI, fill in the correct details, and press the convert button. The plugin should close the UI and automatically skip through the drills while retrieving the data necessary for the team training pack (don't press anything while this is happening). Once it's done recording the data, it will stop skipping through the drills and a toast notification will display saying it's completed (if you have toast notifications enabled). If you bring up the plugin's UI, your pack should now show in the pack selection tab.

Defense only training packs do not work right now. These may or may not be supported in a future update.

# Changelog

v0.2.4
* Fixed bindings not resetting when leaving freeplay/unloading plugin after loading a pack
* Bindings will no longer be set when a pack fails to load
* Added more checks to prevent issues when commands are misused

v0.2.3
* Added some checks to prevent crashes due to misuse
* Fixed drill randomization
* Scoring now advances to the next drill, using shot reset button resets the drill

v0.2.2
* Added/fixed defenders in packs for loading and creating packs
* Fixed crash when pack's description or creator contains an apostrophe
* Block creation of packs with no offensive players

v0.2.1
* Disabled defensive players for conversion, as it is broken right now
* Fixed crash when converting from unpublished custom training pack

v0.2.0
* Added new UI for pack selection, creation, player role assignments, and modifying cooldown and randomization settings
* Custom training pack conversion into team training pack is fully automated now (requires no user input for ball trajectory)
* Upgraded training pack format to include custom training pack code, creator name, and version number

v0.1.0
* Initial release, simply updated from old plugin to 64-bit

# Contact

* [@PenguinDaft](twitter.com/PenguinDaft)
* Discord: DaftPenguin#5103