# Phantom
![Version: 1.9.2](https://img.shields.io/badge/Version-1.9.2-white.svg)
![License: GPL-2.0](https://img.shields.io/badge/License-GPL%202.0-blue.svg)

## About
### Source code for **Phantom ServerSide** GUI

#### Phantom was a server-side made back in 2018 *(Formally known as "BruhK3K" at the time)*.
It has since been discontinued, and I decided to release the source code to the GUI.
Sometime in 2024 I began updating Phantom's GUI more regularly, and it's now become a sort of passion project.
#### Update *(May 14th, 2025)*:
Phantom Version 1.9.2 will most likely be the final version. *Bug Fixes Excluded*

#### Notice
Older version of Phantom may contain bugs that hinder the user experience. Please consider using the [newest version](./Phantom.rbxm).

## License
### This project is licensed under the GNU General Public License v2.0
See the [LICENSE](./LICENSE.txt) file for details.

---

# Changelog

## [Version 1.9.2](https://github.com/FlowScript/Phantom/commit/2fbe1773e953ebcae742603b32aa551bdad7e8be)

**New Features:**
- Added optional `Player(s)` argument to `CopyTools` command

Removed:
- `CopyToolsTo` command

Changes:
- Every other row in the `Actions` Page has a different `Background Color` for better visibility
- GUI Tweaks and Changes

**Bug Fixes**

---

## [Version 1.9.1](https://github.com/FlowScript/Phantom/commit/f05bb334433842746a4c62b420df20d121b62bae)

**New Features:**
- Added `Target Tags` to `Script Hub Player Search` and to `Character`, `SpawnPoint`, `Teleport`, commands
- Added `Team Index` to `Target Tags`
- Added `Ignore Invalid Targets` Setting

**Changes:**
- Changed `AutoR6` Setting to `Auto Convert`
  - `Auto Converts` the Local Player's `Character` to `R6` or `R15`
- Tweaks and Improvements

**Bug Fixes**

---

## [Version 1.9.0](https://github.com/FlowScript/Phantom/commit/3eb91f23fc0cf5e4e5f6c9eb63514e7972f2d0c8)

**New Features:**
- Added targeting Players within a specified Stud radius
  - Example: `kill !10` - kills Players within a 10 Stud radius
- Added Aliases for `!viewing` and `!targets` Tags:
  - `!viewing`: `!view`, `!v`
  - `!targets`: `!target`, `!t`
- Added `UnGear` command
- Added optional `ToolName` argument to the `RemoveTools` command
- Added optional `MaxSpeed` and `Multiple` arguments to the `Car` command
- Added optional `Strength` argument to `Fling` command
- Added optional `SingleTool` argument to multiple *Gear Type* commands
- Added optional `ImageID` and `SoundID` arguments to the `Crash` command
- Added optional `Heat` argument to `Fire` command
- Added optional `Size` argument to `Smoke` command
- Added optional `BrickColorIndex` argument to `Fire`, `Smoke`, and `Sparkles` commands

**Changes:**
- Gears added via the `Gear` command can now be removed using the `UnGear` command
- The `SpawnPoint` command now uses the Targeted Player's Position if no Secondary Target is specified
- Updated the Freecam Script to the latest Roblox Release
  - The `FreeCam` command now has a Keybind Toggle *(Shift + P)*
- Added `R15` Tag as an option to `Script Hub` scripts
- Small Tweaks and Improvements

**Bug Fixes**

---

## [Version 1.8.9](https://github.com/FlowScript/Phantom/commit/315abce3163a441a2baf427e858cf86e68ace22f)

**New Commands:**
- `LocalLoadString`
- `Targets`

**Changes:**
- Command `DecalIDs` and `SoundIDs` are now loaded from `Pastebin` *(Just like Script Hub)*
- `Place` command now has an optional `JobID` Argument
- Small Tweaks and Improvements

**Bug Fixes**

---

## [Version 1.8.8](https://github.com/FlowScript/Phantom/commit/eaceb22a9ccc9f9bbd52835d9f5d111ce14b5ead)

**New Commands:**
- `Decal`, `UnDecal`
- `Insert`, `UnInsert`
- `PlayerList`, `UnPlayerList`
- `PreivousError`, `PreviousSuccess`
- `LoadString`
- `SetTargets`

**New Features:**
- Commands can now be executed on "!targets" after setting Targets with the `SetTargets` command
- Added a Log Client Console Setting for better tracking
- Enhanced Command Search functionality for improved user experience
- Introduced Searching by Type on the Logs page (Valid searches: `type:server`, `client`, `error`, `warning (warn)`, `output (print)`)
- The Script Hub now utilizes "me" instead of the Local Player Name for targeting
- Local Player targeting in Commands and Script Hub is now exclusively done using "me" or "all" (the Local Player's Name will no longer be accepted)
- A warning has been added for executing scripts on multiple players in the Script Hub

**Changes:**
- `Viewing` a Player will now `Persist` if the Character is `Reloaded`
- Small Tweaks and Improvements

**Bug Fixes**

---

## [Version 1.8.7](https://github.com/FlowScript/Phantom/commit/79258b0383fa025e7d22f922c0a7647ab45f4f09)

**New Settings:**
- `Hide Require Logs on Execute`
- `ESP Use Highlight`
- `Translation Styles`

**New Features:**
- A Notification is now displayed when a Require is logged on the Logs page.

**Changes:**
- Small UI Tweaks

**Bug Fixes**

---

## [Version 1.8.6](https://github.com/FlowScript/Phantom/commit/b9df360af7a7c75cf25d499b0fa81b5427b47ef8)

**New Commands:**
- `SpawnPoint`, `UnSpawnPoint`
- `Countdown`, `PrivateCountdown`
- `UnCountdown`, `UnJumpscare`
- `RenameTeam`

**New Features:**
- Script Hub now hides `Requires` from the Console
- Added `Print to Console` setting in Settings Page under `Notifications`
- `Right Clicking` the `Pause Button` while viewing `Console Logs` now restores `Previous Server Logs` using Log History

**Changes:**
- Added `BrickColorIndex` option to more Commands
- Added optional `Everything` tag to the `Clear` Command
- `Server Uptime` is now displayed in a different format

**Bug Fixes**

---

## [Version 1.8.5](https://github.com/FlowScript/Phantom/commit/19075b85799e77adada6f62e51071795fda2acc0)

**New Features:**
- You can now select the `Player` you're currently viewing by using `!viewing`
  - Example: `kill !viewing`
- Added a `Notification` Section in the Settings page
  - Enable or Disable Notifications
  - Enable or Disable `Extra Command Notifications`
  - Change the `Maximum` number of Notifications

**Changes:**
- Reworded several Notifications

**Bug Fixes**

---

## [Version 1.8.4](https://github.com/FlowScript/Phantom/commit/532e99de56668c58b1fd7896d596d053ee71481b)

**New Commands:**
- `Sign`, `UnSign`,
- `Clear`

**New Features:**
- You can now select `Players` in a specific `Team` to run Commands on using the `#` Tag
  - Example: `kill #TeamName`

**Changes:**
- The `CreateTeam` Command now sets the New Team's `AutoAssignable` value to `false`
- Other Small Changes

---

## [Version 1.8.3](https://github.com/FlowScript/Phantom/commit/8823c29223d8fd418a484b1518062de61a7c4534)
**New Features:**
- Added `excludeLocalPlayer` tag for the following Commands:
  - `ban`
  - `apiBan`
  - `kick`
  - `crash`
  - This prevents the Command from running on the Local Player

**New Features:**
- `ForceApiBan` command now accepts UserIDs
- The `View` command now sets the Local Player's `ReplicationFocus` to the player they're viewing

**Changes:**
- Small Notification Changes

---

## [Version 1.8.2](https://github.com/FlowScript/Phantom/commit/0294bdae170d7734e378a40ce255d127cb348789)
**New Commands:**
- `Mine`, `UnMine`
- `Bomb`, `UnBomb`
- `Trap`, `UnTrap`
- `PrivateNotification`

**New Features:**
- Added `ESP` Section in Settings page with Settings:
  - `Toggle`
  - `Display Names`
  - `Use Team Color`
- Notifications can now have different `Duration` times
- Notifications now display a `Progress Bar` indicating the time until the notification disappears

**Changes:**
- Max notification count is now `4` instead of `3`
- Notifications now stay on screen for a default of `5` seconds instead of `10`

**Bug Fixes**

---

## [Version 1.8.1](https://github.com/FlowScript/Phantom/commit/747d7fc229c5a1352aba424dfddaec33850ecdbb)
**New Commands:**
- `ApiBan`, `UnApiBan`, `ForceApiBan`

**New Features:**
- ScriptHub Backup Scripts now immediately load in, in case HTTP requests are put into long queues
- Added ESP toggle and Keybind to the Settings page
- Features and Keybinds have been grouped in the Settings page
- Added optional `Hidden` argument to the `ForceField` command
- Using the `random` tag when specifying a target now excludes the local player (unless they're the only player in the server)

**Bug Fixes**

---

## [Version 1.8.0](https://github.com/FlowScript/Phantom/commit/a7c8434ff200ffef6aea4c1dab5b49429954a96e)
**New Commands:**
- `Bans`, `ForceBan`
- `Guis`, `UnGuis`
- `Inventory`, `UnInventory`

**New Features:**
- Added optional `BrickColorIndex` argument for the following commands: `title`, `hologram`, `createteam`
- Made titles half the size of holograms

**Removed:**
- Deprecated `LegacyChatService` support

**Bug Fixes**

---

## [Version 1.7.9](https://github.com/FlowScript/Phantom/commit/ae75dd50f97e75bb7e00078288e4c1250698ca55)
**Changes:**
- `Change`, `Team`, and `RemoveTeam` commands now support using indexes instead of names
- `Change` command now supports `BoolValues`

**Bug Fixes**

---

## [Version 1.7.8](https://github.com/FlowScript/Phantom/commit/39624e4a86dd90468e68fe9610c27c992d42be0c)
**New Commands:**
- `Title`, `UnTitle`
- `Hologram`, `UnHologram`

**Changes:**
- Updated the look of the Commands Page command bar
- In the Scan page, if the Local Player has the same GUI as the template, the copy button’s image color is set to gray

**Bug Fixes**

---

## [Version 1.7.7](https://github.com/FlowScript/Phantom/commit/64f483fa86626c619584f9a759ae6abfad15e2e4)
**New Commands:**
- `Fog`, `UnFog`
- `MusicCharacter`, `UnMusicCharacter`
- `MusicPart`, `UnMusicPart`
- `ServerLock`, `UnServerLock`
- `UnTeam`

**Changes:**
- Updated how command aliases are rendered
- Added support for multiple commands in a single line (e.g., `command1 args1|command2 args2`)

---

## [Version 1.7.6](https://github.com/FlowScript/Phantom/commit/b39fb87c53073f4fac00805b52b1cf8a18582e80)
**New Features:**
- Added `Copy All Unique` button to Scan page
- Added more actions and notifications
- Cleaned up notifications
- Multiple random players in a command now listed in a single notification
- Notification text is now selectable and copyable
- `Character` and `UnCharacter` commands now apply a `HumanoidDescription` instead of refreshing the character
- You can now use table indices for `DecalIDs` or `SoundIDs` in commands like `Music`, `Jumpscare`, and `SkyBox`

**Bug Fixes**

---

## [Version 1.7.5](https://github.com/FlowScript/Phantom/commit/4e25677d02aec08e82e40ec46cb7e96077aa76de)
**New Features:**
- Added `UnName` command
- Added `Copy` button to Items in Scan page
- Added more custom images
- Added image pre-loading in Intro

---

## [Version 1.7.4](https://github.com/FlowScript/Phantom/commit/5499706bf3375e3719ddc1ac3fbce96935c3f531)
**New Features:**
- Added `Skybox` command with optional default `Image ID`
- Increased default Image IDs to 85 decals
- `Music` command now supports optional `Volume` and `Pitch` arguments and defaults to a provided Sound ID
- `Fire` command now has an optional `Size` argument
- Added 22 default Sound IDs

---

## [Version 1.7.3](https://github.com/FlowScript/Phantom/commit/eba608bc7acacf0c8d5042df74a11934b3f8be55)
**Changes:**
- Made console logs into text boxes to allow text copying (right-click to delete doesn't work for console logs)
- Removed bar color for Chat logs since the new `TextChatService` doesn’t specify whisper/team messages
- Updated how some colors are handled

---

## [Version 1.7.2](https://github.com/FlowScript/Phantom/commit/df20ce93a9cff3209662600831839650c40801e2)
**New Features:**
- Added `PrivateHint` command
- Server page now fetches players from the server and handles templates locally
- Added new icons to Server, Actions, and Scan pages (LocalPlayer, Developer, DeveloperFriend, Hidden, UnHidden)
- `Car` command now places the car in workspace instead of inside the character (a script inside the model will remove it if the player leaves)

---

## [Version 1.7.1](https://github.com/FlowScript/Phantom/commit/7fe9decc6a8f5bffef47db03214606d012c08482)
**New Commands**:
- `StarterGear`, `RemoveStarterGear`
- `Hint`

**New Features:**
- Improved Executor syntax performance

**Bug Fixes:**
- Fixed bug in `Hide` command
- Fixed formatting bug in `Chat` command

---

## [Version 1.7.0](https://github.com/FlowScript/Phantom/commit/2b73e4f93fa3268642d04182ec8eda67f8055fd5)
**Reworks:**
- Reworked the Commands Script and command handling
- Commands now use `DisplayName` by default (use `@` before player name to search by `player.Name`)

**New Commands:**
- `SellAsset`, `SellGamePass`
- `Car`, `UnCar`
- `Gun`, `UnGun`
- `Message`, `Notify`
- `Place`
- `Teleport`
- `CopyToolsTo`
- `Stats`

**Changes:**
- Added more command aliases
- Redesigned Announcements
- `Character` command now supports `DisplayNames` and using `"me"`
- Made `Chat` command use `SendAsync` instead of `DisplaySystemMessage` for more realistic messaging
- `God` command now sets `Humanoid Health` and `MaxHealth` to `math.huge` instead of an invisible forcefield
- `CopyTools` command now has an optional `CopyDuplicates` argument
- `Explode` command now has an optional `Size` argument
- Improved player teleportation

**Bug Fixes**

---

## [Version 1.6.9](https://github.com/FlowScript/Phantom/commit/3c081f976e76b76652ea673c2b2c6295717b9534)
**New Features:**
- Added `R15` command
- Command history now restores typed text when cycling through history with arrow keys

---

## [Version 1.6.8](https://github.com/FlowScript/Phantom/commit/4c36daaf709ee668c9e556e80a426e9a5f99bcf3)
**New Features:**
- Added `Minimize`, `Command Bar`, and `Inspect Sections` to settings
- Added `Use Display Name` setting to Command Bar section
- Execute commands on all, others, or random players by separating them with commas (e.g., `all,all,all,all`)
- Execute commands on a random player in Script Hub by typing `random` into the player box

**Bug Fixes**

---

## [Version 1.6.7](https://github.com/FlowScript/Phantom/commit/438355cf68eea5ea97eca1ae21d5d0d5cd8b165b)
**New Commands:**
- `Hide`, `UnHide`

**Changes:**
- Owner now appears on top in Server page
- Removed command aliases `b` & `k`

**Bug Fixes**

---

## [Version 1.6.6](https://github.com/FlowScript/Phantom/commit/449d6b41d880f7d4a8867cfc7c964086440efa93)
**Changes:**
- Moved Settings to Items Module
- Moved `R6` function to Items Module
- Added `Use Display Name` and `Use Team Color` settings to Settings page
- Added `Chat Logs` section to Settings page
- Removed `Translation Styles`
- Other small changes

---

## [Version 1.6.5](https://github.com/FlowScript/Phantom/commit/ee3f9dc2c9431eca51e1c76ddcb06a7f6ddd9228)
**New Commands:**
- `Ban`, `UnBan`
- `Crash`

**New Features:**
- Added `Ban` command button to Inspect Menu
- `Jumpscare` command now uses a random image if no image is provided
- Toggled state for items in Scan page now auto-updates when changed externally
- Scan page items are now smaller (60 units -> 40 units)
- Items are now ordered by `ClassName` in the Scan page
- Players are now ordered by `Name` in the Server page
- Removed message cap from Logs
- Optimized event connections and disconnections

**Bug Fixes**

---

## [Version 1.6.4](https://github.com/FlowScript/Phantom/commit/426887e216dd26771f652ab8c240a503c068625c)
**Changes:**
- New Script Hub format supporting an infinite number of groups with custom colors
- Added `MouseButton1Click` function to chat logs to toggle between `DisplayName` and `Name`
- Error notification now shows if R6 fails to load when executing a script that requires R6

---

## [Version 1.6.3](https://github.com/FlowScript/Phantom/commit/90b947bf0fe14ba82b5eb930b0b55ec84690acaa)
**Changes:**
- Small UI updates and improvements

**Bug Fixes**

---

## [Version 1.6.2](https://github.com/FlowScript/Phantom/commit/3a0043453f761b6ed2feb68d25b94191f31d6f4a)
**Changes:**
- `F3X` and `Sword` items now cannot be dropped
- Added more checks to music-type commands
- Fixed a bug in the Logs script related to clearing incorrect entries
- Fixed a bug where `local plr = script:FindFirstAncestorWhichIsA("Player")` would be overwritten
- Fixed a bug in the `Chat` command that used `player.Name` instead of `player.DisplayName`
- Fixed a bug where skipping the Announcement would leave it frozen on screen

**Bug Fixes**

---

## [Version 1.6.1](https://github.com/FlowScript/Phantom/commit/1a03e0fe5d9674689b48385d7014c46ba24e8e96)
**New Features:**
- Added `Translation Styles`

**Bug Fixes**

---

## [Version 1.6.0](https://github.com/FlowScript/Phantom/commit/44ec7b9ca38a2379eff39f78b41d0fe0f748eca8)
**New Features:**
- Added `NowPlaying` command
- Added button to switch between `Console` and `Chat` logs
- Added `[Hidden]` argument to `BTools` command
- Added `Translate Chat Logs` setting to Settings page
- Added `Reset Mouse Icon` setting to the Settings page
- Added `Developer Icon` next to Game Developer's name in the Server, Action, Scan, and Inspect pages

**Changes:**
- Renamed `Console` page to `Logs`

**Bug Fixes**

---

## [Version 1.5.8](https://github.com/FlowScript/Phantom/commit/a70b2afd4083b84b8feddae33a6c9f6f776272cf)
**New Features:**
- Added client execute for the executor
- Custom notifications UI
- Notifications for errors and invalid commands
- Added `system` command
- Updated backup `scriptHub` scripts
- Other small changes

**Bug Fixes**

---

## [Version 1.5.7](https://github.com/FlowScript/Phantom/commit/1a39e4c3a127f5d2d9fe62a8b8b6a3facbb558f4)
**New Features:**
- Added `ClickTP` command
- Added more scripts to `scriptHub`

**Removed:**
- `Kidnap` and `Guns` commands

**Changes:**
- Fixed bugs with `R6`
- `R6` is now a local module instead of a require
- `ScriptHub` is now server-side instead of client-side

---

## [Version 1.5.6](https://github.com/FlowScript/Phantom/commit/c486bbdb6271b951394a2b00c0f8ee6f60428fa8)
**Removed:**
- Removed the home page

**Changes:**
- Completely redesigned the commands script
- Added better formatting for Server, Scan, and Actions pages
- Added visibility toggle in Scan page for `ScreenGUIs`, `Scripts`, and `LocalScripts`
- Changed some styling for the Settings page

---

## [Version 1.5.5](https://github.com/FlowScript/Phantom/commit/ad7e8da623ac997cdfbc4200294cd320d3fc02c7)
**New Features:**
- Added search functionality to console
- Added `Jumpscare` command
- Removed unused objects

**Bug Fixes**

---

## [Version 1.5.4](https://github.com/FlowScript/Phantom/commit/98511975ce0eb8767d9eeea630a272e90a08c2e6)
**Changes:**
- `Script Hub` now loads from URL
- Other small changes

---

## [Version 1.5.3](https://github.com/FlowScript/Phantom/commit/dbbe59b769be68420f10417b6a48a5abcfe91265)
**Changes:**
- Script Hub script changes
- Small tweaks and bug fixes

---

## [Version 1.5.2](https://github.com/FlowScript/Phantom/commit/295e53a1afca2c6e213b54cf23d635dc716ec31f)
**Bug Fixes:**
- Fixed `Server Page Search`

---

## [Version 1.5.1](https://github.com/FlowScript/Phantom/commit/b3fbafeeb2ec954e0c67daf4dbba53df139edf03)
**Changes:**
- `Script Hub` fixes

---

## [Version 1.5.0](https://github.com/FlowScript/Phantom/commit/ab1b65c31cb0b097aee051adf148ea9c8f047eeb)
**Changes:**
- Command history changes
- New setting added

**Bug Fixes**

---

## [Version 1.4.9](https://github.com/FlowScript/Phantom/commit/47dbe1bc04768d8934ccd3a6cf8fc18667ee63bf)
**Changes:**
- Changed `Script Hub` search
- Made command history longer

**Bug Fixes**

---

## [Version 1.4.8](https://github.com/FlowScript/Phantom/commit/54d9cda30ec71b4382c5f253fc88b6d4d8d98a3b)
**Bug Fixes**

---

## [Version 1.4.7](https://github.com/FlowScript/Phantom/commit/9a75751904c7fda371c2fff81654459b543d8b91)
**Bug Fixes:**
- Fixed bugs related to the action page

---

## [Version 1.4.6](https://github.com/FlowScript/Phantom/commit/e459cb40a8fababc441de9d8133519bcc6036758) and Lower
**Unknown Changes**