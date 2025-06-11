# Changelog

## [Version 1.9.2 (Latest)](https://github.com/FlowScript/PHANTOM/commit/8f9c6e59a1f52fc6fc500baed9e57fe737e815c8)

**New Commands:**
- `Punish`, `UnPunish`
- `Accessory`, `UnAccessory`
- `MeshAccessory`, `UnMeshAccessory`
- `Mesh`, `UnMesh`
- `Blur`, `UnBlur`
- `ColorCorrection`, `UnColorCorrection`
- `LocalBlur`, `UnLocalBlur`
- `LocalColorCorrection`, `UnLocalColorCorrection`
- `LocalMusic`, `UnLocalMusic`
- `ScreenShake`, `UnScreenShake`
- `FakeAnnounceMent`
- `FakeMessage`
- `PrivateFakeChat`
- `PrivateSystemMessage`
- `Face`, `UnFace`
- `Shirt`, `UnShirt`
- `Pants`, `UnPants`
- `UnMusic`, `UnSkyBox`
  - *`Music 0` and `SkyBox 0` Still Work*
  - *These Commands Where Added to Prevent Confusion*

**New Optional Arguments for Commands:**
- `Player(s)` to the `CopyTools` command
- `ToolName` to the `StarterGear`, `RemoveStarterGear`, `UnGear`, `CopyTools` commands
- `StarterGear`, `Droppable`, and `AutoEquip` to all *Gear Type* commands
- `AutoAssignable` to the `CreateTeam` and `RenameTeam` commands
- `DoubleSided` to the `Decal` and `Sign` commands
- `BlastPressure` and `BrickColorIndex`*2* to the `Explode` command
- `MaxDistance` to the `MusicCharacter` and `MusicPart` commands
- `AddNew` to the `Music` command
- `Volume` and `Pitch` to the `JumpScare` and `Crash` commands
- `Player` to the `NowPlaying` command
- `ForceFieldDuration` to the `SpawnPoint` command
- `CelestialBodies` to the `Skybox` command
- `Opacity` to the `Smoke` command

**New Features:**
- Added `Target Exclusion` with `-`
  - Example: `kill all,-player2` - This will kill `All` players besides `Player2`
- Added `Refresh` button to the `Script Hub`
- `Distance Tag` now uses `Viewing` Player if a Player is being `Viewed`
- You can now view your `Local GUIs` by `Scanning the Local Player`
- The `Scan` page now tracks Items' `Names` and will Update them
- Added `Type Searching` to the `Scan` page
  - Example: `type:script ScriptName`, `type:script,screengui`
- Added `High Priority Keybinds` setting
  - When enabled, PHANTOM will use `ContextActionService` instead of `UserInputService` to handle Keybinds
- The `Logs` page will now display the `Current Number` of Console Logs and Chat Logs
- Improved `All` Search Functions
  - `Position Saving` and `Multi Searching`
  - Multi Search Example: `search1,search2,etc...`
- Added support for more `Strings` and `Comments` in Executor Syntax
  - `[[ ]]`, `[=[ ]=]`, `--[[ ]]`, `--[=[ ]=]`
- Added `Notifications` for `Log Restore`

**Removed:**
- `CopyToolsTo`, `Fog`, `UnFog`, `PreviousError`, `PrivousSuccess` commands
- `Hide Require Logs on Execute` and `Reset Mouse Icon` settings *(Now Enabled by Default)*

**Changes:**
- Reduced GUI `Padding` from `10` to `5`
- Every other row in the `Actions` page has a different `Background Color` for better visibility
- `Command History` is now synced between the `Commands Page` and the `Command Bar`
- Slightly Changed the Look of the `Other Pages`
- Changed how the `Name` script functions
- Tweaks and Changes to `GUI` and `Backend`

**Bug Fixes**

---

## [Version 1.9.1](https://github.com/FlowScript/PHANTOM/commit/f05bb334433842746a4c62b420df20d121b62bae)

**New Features:**
- Added `Target Tags` to the `Script Hub Player Search`, and to the `Character`, `SpawnPoint`, and `Teleport` commands
- Added `Team Index` to `Target Tags`
- Added `Ignore Invalid Targets` setting

**Changes:**
- Changed `AutoR6` setting to `Auto Convert`
  - `Auto Converts` the Local Player's `Character` to `R6` or `R15`
- Tweaks and Improvements

**Bug Fixes**

---

## [Version 1.9.0](https://github.com/FlowScript/PHANTOM/commit/3eb91f23fc0cf5e4e5f6c9eb63514e7972f2d0c8)

**New Features:**
- Added targeting Players within a specified `Stud Radius`
  - Example: `kill !10` - kills Players within a 10 Stud radius
- Added Aliases for `!viewing` and `!targets` Tags:
  - `!viewing`: `!view`, `!v`
  - `!targets`: `!target`, `!t`
- Added `UnGear` command
- Added optional `ToolName` argument to the `RemoveTools` command
- Added optional `MaxSpeed` and `Multiple` arguments to the `Car` command
- Added optional `Strength` argument to the `Fling` command
- Added optional `SingleTool` argument to multiple *Gear Type* commands
- Added optional `ImageID` and `SoundID` arguments to the `Crash` command
- Added optional `Heat` argument to the `Fire` command
- Added optional `Size` argument to the `Smoke` command
- Added optional `BrickColorIndex` argument to the `Fire`, `Smoke`, and `Sparkles` commands

**Changes:**
- Gears added via the `Gear` command can now be removed using the `UnGear` command
- The `SpawnPoint` command now uses the Targeted Player's Position if no Secondary Target is specified
- Updated the Freecam Script to the latest Roblox Release
  - The `FreeCam` command now has a Keybind Toggle *(Shift + P)*
- Added `R15` Tag as an option to the `Script Hub` scripts
- Small Tweaks and Improvements

**Bug Fixes**

---

## [Version 1.8.9](https://github.com/FlowScript/PHANTOM/commit/315abce3163a441a2baf427e858cf86e68ace22f)

**New Commands:**
- `LocalLoadString`
- `Targets`

**Changes:**
- Command `DecalIDs` and `SoundIDs` are now loaded from `Pastebin` *(Just like Script Hub)*
- `Place` command now has an optional `JobID` Argument
- Small Tweaks and Improvements

**Bug Fixes**

---

## [Version 1.8.8](https://github.com/FlowScript/PHANTOM/commit/eaceb22a9ccc9f9bbd52835d9f5d111ce14b5ead)

**New Commands:**
- `Decal`, `UnDecal`
- `Insert`, `UnInsert`
- `PlayerList`, `UnPlayerList`
- `PreivousError`, `PreviousSuccess`
- `LoadString`
- `SetTargets`

**New Features:**
- Commands can now be executed on "!targets" after setting Targets with the `SetTargets` command
- Added `Log Client Console` setting for better tracking
- Improved `Command` search for better results
- Introduced Searching by Type on the `Logs` page *(Valid searches: `type:server`, `client`, `error`, `warning (warn)`, `output (print)`)*
- The `Script Hub` now uses `me` instead of the `Local Player` Name for `Targeting`
- `Local Player` Targeting in the `Commands` and `Script Hub` pages is now done using `me` or `all` *(The Local Player's Name will no longer be accepted)*
- A `Warning` has been added for executing scripts on `Multiple` Players in the `Script Hub`

**Changes:**
- `Viewing` a Player will now `Persist` if the Character is `Reloaded`
- Small Tweaks and Improvements

**Bug Fixes**

---

## [Version 1.8.7](https://github.com/FlowScript/PHANTOM/commit/79258b0383fa025e7d22f922c0a7647ab45f4f09)

**New Settings:**
- `Hide Require Logs on Execute`
- `ESP Use Highlight`
- `Translation Styles`

**New Features:**
- A `Notification` is now displayed when a `Require` is logged on the `Logs` page

**Changes:**
- Small UI Tweaks

**Bug Fixes**

---

## [Version 1.8.6](https://github.com/FlowScript/PHANTOM/commit/b9df360af7a7c75cf25d499b0fa81b5427b47ef8)

**New Commands:**
- `SpawnPoint`, `UnSpawnPoint`
- `Countdown`, `PrivateCountdown`
- `UnCountdown`, `UnJumpscare`
- `RenameTeam`

**New Features:**
- `Script Hub` now hides `Requires` from the Console
- Added `Print to Console` setting to the `Settings` page under `Notifications`
- `Right Clicking` the `Pause Button` while viewing `Console Logs` now restores `Previous Server Logs` using Log History

**Changes:**
- Added `BrickColorIndex` option to more Commands
- Added optional `Everything` tag to the `Clear` Command
- `Server Uptime` is now displayed in a different format

**Bug Fixes**

---

## [Version 1.8.5](https://github.com/FlowScript/PHANTOM/commit/19075b85799e77adada6f62e51071795fda2acc0)

**New Features:**
- You can now select the `Player` you're currently viewing by using `!viewing`
  - Example: `kill !viewing`
- Added a `Notification` Section to the `Settings` page
  - Enable or Disable `Notifications`
  - Enable or Disable `Extra Command Notifications`
  - Change the `Maximum` number of `Notifications`

**Changes:**
- Reworded several `Notifications`

**Bug Fixes**

---

## [Version 1.8.4](https://github.com/FlowScript/PHANTOM/commit/532e99de56668c58b1fd7896d596d053ee71481b)

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

## [Version 1.8.3](https://github.com/FlowScript/PHANTOM/commit/8823c29223d8fd418a484b1518062de61a7c4534)
**New Features:**
- Added `excludeLocalPlayer` tag for the following Commands:
  - `ban`
  - `apiBan`
  - `kick`
  - `crash`
  - This prevents the `Command` from running on the `Local Player`

**New Features:**
- `ForceApiBan` command now accepts UserIDs
- The `View` command now sets the Local Player's `ReplicationFocus` to the player they're `Viewing`

**Changes:**
- Small Notification Changes

---

## [Version 1.8.2](https://github.com/FlowScript/PHANTOM/commit/0294bdae170d7734e378a40ce255d127cb348789)
**New Commands:**
- `Mine`, `UnMine`
- `Bomb`, `UnBomb`
- `Trap`, `UnTrap`
- `PrivateNotification`

**New Features:**
- Added `ESP` Section to the `Settings` page with Settings:
  - `Toggle`
  - `Display Names`
  - `Use Team Color`
- `Notifications` can now have different `Duration` times
- `Notifications` now display a `Progress Bar` indicating the time until the notification disappears

**Changes:**
- Max notification count is now `4` instead of `3`
- Notifications now stay on screen for a default of `5` seconds instead of `10`

**Bug Fixes**

---

## [Version 1.8.1](https://github.com/FlowScript/PHANTOM/commit/747d7fc229c5a1352aba424dfddaec33850ecdbb)
**New Commands:**
- `ApiBan`, `UnApiBan`, `ForceApiBan`

**New Features:**
- `Script Hub` Backup Scripts now immediately load in *(In case HTTP requests are put into long queues)*
- Added `ESP toggle` and `Keybind` to the `Settings` page
- `Features` and `Keybinds` have been grouped in the `Settings` page
- Added optional `Hidden` argument to the `ForceField` command
- Using the `Random` tag when specifying a target now excludes the local player *(Unless they're the only player in the server)*

**Bug Fixes**

---

## [Version 1.8.0](https://github.com/FlowScript/PHANTOM/commit/a7c8434ff200ffef6aea4c1dab5b49429954a96e)
**New Commands:**
- `Bans`, `ForceBan`
- `Guis`, `UnGuis`
- `Inventory`, `UnInventory`

**New Features:**
- Added optional `BrickColorIndex` argument for the following commands: `Title`, `Hologram`, `CreateTeam`
- Made `Titles` half the size of `Holograms`

**Removed:**
- Deprecated `LegacyChatService` support

**Bug Fixes**

---

## [Version 1.7.9](https://github.com/FlowScript/PHANTOM/commit/ae75dd50f97e75bb7e00078288e4c1250698ca55)
**Changes:**
- `Change`, `Team`, and `RemoveTeam` commands now support using `Indexes` instead of `Names`
- `Change` command now supports `BoolValues`

**Bug Fixes**

---

## [Version 1.7.8](https://github.com/FlowScript/PHANTOM/commit/39624e4a86dd90468e68fe9610c27c992d42be0c)
**New Commands:**
- `Title`, `UnTitle`
- `Hologram`, `UnHologram`

**Changes:**
- Updated the look of the `Command Bar` in the `Commands` page
- In the `Scan` page, if the `Local Player` has the same GUI as the template, the copy button’s image color is set to gray

**Bug Fixes**

---

## [Version 1.7.7](https://github.com/FlowScript/PHANTOM/commit/64f483fa86626c619584f9a759ae6abfad15e2e4)
**New Commands:**
- `Fog`, `UnFog`
- `MusicCharacter`, `UnMusicCharacter`
- `MusicPart`, `UnMusicPart`
- `ServerLock`, `UnServerLock`
- `UnTeam`

**Changes:**
- Updated how `Command Aliases` are rendered
- Added support for multiple commands *(e.g., `command1 args1|command2 args2`)*

---

## [Version 1.7.6](https://github.com/FlowScript/PHANTOM/commit/b39fb87c53073f4fac00805b52b1cf8a18582e80)
**New Features:**
- Added `Copy All Unique` button to the `Scan` page
- Added more `Actions` and `Notifications`
- Cleaned up `Notifications`
- Multiple `Random` Players in a command now listed in a single `Notification`
- Notification text is now selectable and copyable
- `Character` and `UnCharacter` commands now apply a `HumanoidDescription` instead of refreshing the character
- You can now use table indices for `DecalIDs` or `SoundIDs` in commands like `Music`, `Jumpscare`, and `SkyBox`

**Bug Fixes**

---

## [Version 1.7.5](https://github.com/FlowScript/PHANTOM/commit/4e25677d02aec08e82e40ec46cb7e96077aa76de)
**New Features:**
- Added `UnName` command
- Added `Copy` button to Items in the `Scan` page
- Added more custom images
- Added image pre-loading in Intro

---

## [Version 1.7.4](https://github.com/FlowScript/PHANTOM/commit/5499706bf3375e3719ddc1ac3fbce96935c3f531)
**New Features:**
- Added `Skybox` command with optional default `Image ID`
- Increased default Image IDs to 85 decals
- `Music` command now supports optional `Volume` and `Pitch` arguments and defaults to a provided Sound ID
- `Fire` command now has an optional `Size` argument
- Added 22 default Sound IDs

---

## [Version 1.7.3](https://github.com/FlowScript/PHANTOM/commit/eba608bc7acacf0c8d5042df74a11934b3f8be55)
**Changes:**
- Made console logs into text boxes to allow text copying *(Right-click to delete doesn't work for console logs)*
- Removed bar color for Chat logs since the new `TextChatService` doesn’t specify whisper/team messages
- Updated how some colors are handled

---

## [Version 1.7.2](https://github.com/FlowScript/PHANTOM/commit/df20ce93a9cff3209662600831839650c40801e2)
**New Features:**
- Added `PrivateHint` command
- The `Server` page now fetches players from the server and handles templates locally
- Added new icons to the `Server`, `Actions`, and `Scan` pages *(LocalPlayer, Developer, DeveloperFriend, Hidden, UnHidden)*
- The `Car` command now places the car in workspace instead of inside the character *(A script inside the model will remove it if the player leaves)*

---

## [Version 1.7.1](https://github.com/FlowScript/PHANTOM/commit/7fe9decc6a8f5bffef47db03214606d012c08482)
**New Commands**:
- `StarterGear`, `RemoveStarterGear`
- `Hint`

**New Features:**
- Improved Executor syntax performance

**Bug Fixes:**
- Fixed bug in the `Hide` command
- Fixed formatting bug in the `Chat` command

---

## [Version 1.7.0](https://github.com/FlowScript/PHANTOM/commit/2b73e4f93fa3268642d04182ec8eda67f8055fd5)
**Reworks:**
- Reworked the Commands Script and command handling
- Commands now use `DisplayName` by default *(Use `@` before player name to search by `player.Name`)*

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

## [Version 1.6.9](https://github.com/FlowScript/PHANTOM/commit/3c081f976e76b76652ea673c2b2c6295717b9534)
**New Features:**
- Added `R15` command
- Command history now restores typed text when cycling through history with arrow keys

---

## [Version 1.6.8](https://github.com/FlowScript/PHANTOM/commit/4c36daaf709ee668c9e556e80a426e9a5f99bcf3)
**New Features:**
- Added `Minimize`, `Command Bar`, and `Inspect Sections` to the `Settings` page
- Added `Use Display Name` setting to Command Bar section
- Execute commands on all, others, or random players by separating them with commas *(e.g., `all,all,all,all`)*
- Execute commands on a random player in the `Script Hub` by typing `random` into the player box

**Bug Fixes**

---

## [Version 1.6.7](https://github.com/FlowScript/PHANTOM/commit/438355cf68eea5ea97eca1ae21d5d0d5cd8b165b)
**New Commands:**
- `Hide`, `UnHide`

**Changes:**
- `Owner` now appears on top in the `Server` page
- Removed command aliases `b` & `k`

**Bug Fixes**

---

## [Version 1.6.6](https://github.com/FlowScript/PHANTOM/commit/449d6b41d880f7d4a8867cfc7c964086440efa93)
**Changes:**
- Moved Settings to Items Module
- Moved `R6` function to Items Module
- Added `Use Display Name` and `Use Team Color` settings to the `Settings` page
- Added `Chat Logs` section to the `Settings` page
- Removed `Translation Styles`
- Other small changes

---

## [Version 1.6.5](https://github.com/FlowScript/PHANTOM/commit/ee3f9dc2c9431eca51e1c76ddcb06a7f6ddd9228)
**New Commands:**
- `Ban`, `UnBan`
- `Crash`

**New Features:**
- Added `Ban` command button to Inspect Menu
- `Jumpscare` command now uses a random image if no image is provided
- Toggled state for items in the `Scan` page now auto-updates when changed externally
- `Scan` page items are now smaller *(60 units -> 40 units)*
- Items are now ordered by `ClassName` in the `Scan` page
- Players are now ordered by `Name` in the `Server` page
- Removed message cap from Logs
- Optimized event connections and disconnections

**Bug Fixes**

---

## [Version 1.6.4](https://github.com/FlowScript/PHANTOM/commit/426887e216dd26771f652ab8c240a503c068625c)
**Changes:**
- New `Script Hub` format supporting an infinite number of groups with custom colors
- Added `MouseButton1Click` function to chat logs to toggle between `DisplayName` and `Name`
- Error notification now shows if R6 fails to load when executing a script that requires R6

---

## [Version 1.6.3](https://github.com/FlowScript/PHANTOM/commit/90b947bf0fe14ba82b5eb930b0b55ec84690acaa)
**Changes:**
- Small UI updates and improvements

**Bug Fixes**

---

## [Version 1.6.2](https://github.com/FlowScript/PHANTOM/commit/3a0043453f761b6ed2feb68d25b94191f31d6f4a)
**Changes:**
- `F3X` and `Sword` items now cannot be dropped
- Added more checks to music-type commands
- Fixed a bug in the Logs script related to clearing incorrect entries
- Fixed a bug where `local plr = script:FindFirstAncestorWhichIsA("Player")` would be overwritten
- Fixed a bug in the `Chat` command that used `player.Name` instead of `player.DisplayName`
- Fixed a bug where skipping the Announcement would leave it frozen on screen

**Bug Fixes**

---

## [Version 1.6.1](https://github.com/FlowScript/PHANTOM/commit/1a03e0fe5d9674689b48385d7014c46ba24e8e96)
**New Features:**
- Added `Translation Styles`

**Bug Fixes**

---

## [Version 1.6.0](https://github.com/FlowScript/PHANTOM/commit/44ec7b9ca38a2379eff39f78b41d0fe0f748eca8)
**New Features:**
- Added `NowPlaying` command
- Added button to switch between `Console` and `Chat` logs
- Added `[Hidden]` argument to the `BTools` command
- Added `Translate Chat Logs` setting to the `Settings` page
- Added `Reset Mouse Icon` setting to the `Settings` page
- Added `Developer Icon` next to Game Developer's name in the `Server`, `Action`, `Scan`, and `Inspect` pages

**Changes:**
- Renamed the `Console` page to `Logs`

**Bug Fixes**

---

## [Version 1.5.8](https://github.com/FlowScript/PHANTOM/commit/a70b2afd4083b84b8feddae33a6c9f6f776272cf)
**New Features:**
- Added client execute for the executor
- Custom notifications UI
- Notifications for errors and invalid commands
- Added `system` command
- Updated backup `script Hub` scripts
- Other small changes

**Bug Fixes**

---

## [Version 1.5.7](https://github.com/FlowScript/PHANTOM/commit/1a39e4c3a127f5d2d9fe62a8b8b6a3facbb558f4)
**New Features:**
- Added `ClickTP` command
- Added more scripts to the `script Hub`

**Removed:**
- `Kidnap` and `Guns` commands

**Changes:**
- Fixed bugs with `R6`
- `R6` is now a local module instead of a require
- `Script Hub` is now server-side instead of client-side

---

## [Version 1.5.6](https://github.com/FlowScript/PHANTOM/commit/c486bbdb6271b951394a2b00c0f8ee6f60428fa8)
**Removed:**
- Removed the `Home` page

**Changes:**
- Completely redesigned the commands script
- Added better formatting for the `Server`, `Scan`, and `Actions` pages
- Added visibility toggle in the `Scan` page for `ScreenGUIs`, `Scripts`, and `LocalScripts`
- Changed some styling for the `Settings` page

---

## [Version 1.5.5](https://github.com/FlowScript/PHANTOM/commit/ad7e8da623ac997cdfbc4200294cd320d3fc02c7)
**New Features:**
- Added search functionality to console
- Added `Jumpscare` command
- Removed unused objects

**Bug Fixes**

---

## [Version 1.5.4](https://github.com/FlowScript/PHANTOM/commit/98511975ce0eb8767d9eeea630a272e90a08c2e6)
**Changes:**
- `Script Hub` now loads from URL
- Other small changes

---

## [Version 1.5.3](https://github.com/FlowScript/PHANTOM/commit/dbbe59b769be68420f10417b6a48a5abcfe91265)
**Changes:**
- `Script Hub` script changes
- Small tweaks and bug fixes

---

## [Version 1.5.2](https://github.com/FlowScript/PHANTOM/commit/295e53a1afca2c6e213b54cf23d635dc716ec31f)
**Bug Fixes:**
- Fixed the `Server` page search

---

## [Version 1.5.1](https://github.com/FlowScript/PHANTOM/commit/b3fbafeeb2ec954e0c67daf4dbba53df139edf03)
**Changes:**
- `Script Hub` Fixes

---

## [Version 1.5.0](https://github.com/FlowScript/PHANTOM/commit/ab1b65c31cb0b097aee051adf148ea9c8f047eeb)
**Changes:**
- Command history changes
- New setting added

**Bug Fixes**

---

## [Version 1.4.9](https://github.com/FlowScript/PHANTOM/commit/47dbe1bc04768d8934ccd3a6cf8fc18667ee63bf)
**Changes:**
- Changed `Script Hub` search
- Made command history longer

**Bug Fixes**

---

## [Version 1.4.8](https://github.com/FlowScript/PHANTOM/commit/54d9cda30ec71b4382c5f253fc88b6d4d8d98a3b)
**Bug Fixes**

---

## [Version 1.4.7](https://github.com/FlowScript/PHANTOM/commit/9a75751904c7fda371c2fff81654459b543d8b91)
**Bug Fixes:**
- Fixed bugs related to the `Action` page

---

## [Version 1.4.6](https://github.com/FlowScript/PHANTOM/commit/e459cb40a8fababc441de9d8133519bcc6036758) and Lower
**Unknown Changes**