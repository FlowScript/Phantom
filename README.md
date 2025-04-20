# Phantom
![Version: 1.8.2](https://img.shields.io/badge/Version-1.8.2-white.svg)
![License: GPL-2.0](https://img.shields.io/badge/License-GPL%202.0-blue.svg)

## About
### Source code for **Phantom ServerSide** GUI

#### Phantom was a server-side made back in 2018 *(Formally known as "BruhK3K" at the time)*.
It has since been discontinued, and I decided to release the source code to the GUI.
Sometime in 2024 I began updating Phantom's GUI more regularly, and it's now become a sort of passion project.
#### Update 04/19/25:
Phantom Version 1.8.2 will most likely be the final version. *Bug Fixes Excluded*

#### Notice
Older version of Phantom may contain bugs that hinder the user experience. Please consider using the [newest version](./Phantom.rbxm).

## License
### This project is licensed under the GNU General Public License v2.0
See the [LICENSE](./LICENSE.txt) file for details.

---

# Changelog

## [Version 1.8.2](https://github.com/FlowScript/Phantom/commit/bb5af8b97d254bf3546eac18ad98c71ce116f24a)
**Added Commands:**
- `mine`, `unmine`
- `bomb`, `unbomb`
- `trap`, `untrap`
- `privatenotification`

**New Features:**
- Notifications can now have different `duration` times
- Notifications now display a `progress bar` indicating the time until the notification disappears

**Changes:**
- Max notification count is now `4` instead of `3`
- Notifications now stay on screen for a default of `5` seconds instead of `10`

**Bug Fixes**

---

## [Version 1.8.1](https://github.com/FlowScript/Phantom/commit/747d7fc229c5a1352aba424dfddaec33850ecdbb)
**Added Commands:**
- `apiban`, `unapiban`, `forceapiban`

**New Features:**
- ScriptHub Backup Scripts now immediately load in, in case HTTP requests are put into long queues
- Added ESP toggle and Keybind to the Settings page
- Features and Keybinds have been grouped in the Settings page
- Added optional `Hidden` argument to the `forcefield` command
- Using the `random` tag when specifying a target now excludes the local player (unless they're the only player in the server)

**Bug Fixes**

---

## [Version 1.8.0](https://github.com/FlowScript/Phantom/commit/a7c8434ff200ffef6aea4c1dab5b49429954a96e)
**Added Commands:**
- `bans`, `forceban`, `guis`, `unguis`, `inventory`, `uninventory`

**New Features:**
- Added optional `BrickColorIndex` argument for the following commands: `title`, `hologram`, `createteam`
- Made titles half the size of holograms

**Removed:**
- Deprecated `LegacyChatService` support

**Bug Fixes**

---

## [Version 1.7.9](https://github.com/FlowScript/Phantom/commit/ae75dd50f97e75bb7e00078288e4c1250698ca55)
**Changes:**
- `Change`, `Team`, `RemoveTeam` commands now support using indexes instead of names
- `Change` command now supports `BoolValues`

**Bug Fixes**

---

## [Version 1.7.8](https://github.com/FlowScript/Phantom/commit/39624e4a86dd90468e68fe9610c27c992d42be0c)
**New Commands:**
- Added `Title`, `UnTitle`, `Hologram`, `UnHologram` commands

**Changes:**
- Updated the look of the Commands Page command bar
- In the Scan page, if the Local Player has the same GUI as the template, the copy button’s image color is set to gray

**Bug Fixes**

---

## [Version 1.7.7](https://github.com/FlowScript/Phantom/commit/64f483fa86626c619584f9a759ae6abfad15e2e4)
**Added Commands:**
- `fog`, `unfog`
- `musiccharacter`, `unmusiccharacter`
- `musicpart`, `unmusicpart`
- `serverlock`, `unserverlock`
- `unteam`

**Changes:**
- Updated how command aliases are rendered
- Added support for multiple commands in a single line (e.g., `command1 args1|command2 args2`)

---

## [Version 1.7.6](https://github.com/FlowScript/Phantom/commit/b39fb87c53073f4fac00805b52b1cf8a18582e80)
**New Features:**
- Added `UnName` command
- Added `CopyAllUnique` button to Scan page
- Added more actions and notifications
- Cleaned up notifications
- Multiple random players in a command now listed in a single notification
- Notification text is now selectable and copyable
- `Character` and `UnCharacter` commands now apply a `HumanoidDescription` instead of refreshing the character
- You can now use table indices for `decalIDs` or `soundIDs` in commands like `Music`, `JumpScare`, and `SkyBox`

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
**New Features:**
- Added `Hint`, `StarterGear`, and `RemoveStarterGear` commands
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
- Added `Car`, `UnCar`, `CopyToolsTo`, `Gun`, `UnGun`, `Message`, `Notify`, `Place`, `SellAsset`, `SellGamePass`, `Stats`, `Teleport`

**Other Changes:**
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
- Execute commands on a random player in Script Hub by typing `"random"` into the player box

**Bug Fixes**

---

## [Version 1.6.7](https://github.com/FlowScript/Phantom/commit/438355cf68eea5ea97eca1ae21d5d0d5cd8b165b)
**New Commands:**
- Added `Hide` and `Unhide` commands

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
**New Features:**
- Added `Ban`, `Unban`, and `Crash` commands
- Added `Ban` button to Inspect Menu
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
**Changes:**
- Renamed `Console` page to `Logs`
- Added button to switch between `Console` and `Chat` logs
- Added `NowPlaying` command
- Added `[Hidden]` argument to `BTools` command
- Added `Translate Chat Logs` feature to Settings page
- Added `Reset Mouse Icon` feature to the Settings page
- Added `Developer Icon` next to Game Developer's name in the Server, Action, Scan, and Inspect pages

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
**Changes:**
- Fixed bugs with `R6`
- `R6` is now a local module instead of a require
- `ScriptHub` is now server-side instead of client-side
- Removed `kidnap` and `guns` commands
- Added `clicktp` command
- Added more scripts to `scriptHub`
- And more...

---

## [Version 1.5.6](https://github.com/FlowScript/Phantom/commit/c486bbdb6271b951394a2b00c0f8ee6f60428fa8)
**Changes:**
- Removed the home page (who needed it, right?)
- Completely redesigned the commands script
- Added better formatting for Server, Scan, and Actions pages
- Added visibility toggle in Scan page for `screenguis`, `scripts`, and `localscripts`
- Changed some styling for the Settings page
- Removed some other stuff (can't remember everything!)

---

## [Version 1.5.5](https://github.com/FlowScript/Phantom/commit/ad7e8da623ac997cdfbc4200294cd320d3fc02c7)
**New Features:**
- Added search functionality to console
- Added `jumpscare` command
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