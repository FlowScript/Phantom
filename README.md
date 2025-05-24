# Phantom
![Version: 1.9.2](https://img.shields.io/badge/Version-1.9.2-white.svg)
![License: GPL-2.0](https://img.shields.io/badge/License-GPL%202.0-blue.svg)

## About
### Source code for **Phantom ServerSide** GUI

Phantom was a server-side made back in 2018 *(Formally known as "BRUHK3K" at the time)*.  
It has since been discontinued, and I decided to release the source code to the GUI.  
Sometime in 2024 I began updating Phantom's GUI more regularly, and it's now become a sort of passion project.
#### Update *(May 24th, 2025)*:
There will be no further updates after Version 1.9.2

#### Notice
Older version of Phantom may contain bugs that hinder the user experience. Please consider using the [Newest Version](./Phantom.rbxm).

## License
### This project is licensed under the GNU General Public License v2.0
See the [LICENSE](./LICENSE.txt) file for details.

---

# Pages and Features List
## Executor:
![Executor](./Images/executor.png)
- Code Execution
  - `Client Sided`, `Server Sided`
- Local Player Variable
  - Quickly Reference the `Local Player` by Using the Variable `LPlr`
- Syntax Coloring
- Line Counting

## Script Hub:
![Script Hub](./Images/scriptHub.png)
- Built-In Backup Script List if Download of Pastebin Failed
  - Refresh Option Provided to Try Again
- Version Tracking
- Multiple Script Groups with Custom Colors
  - Differentiate Danger Levels
- Warnings for Executing on Multiple Players
  - Executing on Multiple Players
  - Executing Scripts Marked as Dangerous
- Auto Convert Tags
  - `R6`, `R15`
  - Auto Converts Target on Script Execution if Necessary
- Target Player Variable
  - Quickly Reference the `Target Player` by Using the Variable `LPlr` inside the Script String

## Commands:
![Commands](./Images/commands.png)
- 170 Built-In Commands
- Command Aliases
- Optional Command Arugments
- Advanced Player Targeting
  - Special Targets: `me`, `all`, `others`, `random`, `!viewing`, `!targets`, `!distance`, `#team`
  - Target Exclusion: `-playerName`, `-me`, `-others`, `-random`, `-!viewing`, `-!targets`, `-!distance`, `#team`
- Command History
  - Use the `Up` and `Down` Arrow Keys to Navigate the Command History

## Command Bar:
![Command Bar](./Images/commandBar.png)
- Quickly Execute Scripts by Pulling Up the Command Bar
  - Default Keybind: `;`
- Command List

## Logs:
![Logs](./Images/logs.png)
- Console Logs
  - `Client`, `Server`
  - `Outputs`, `Warnings`, `Errors`
- Chat Logs
  - `Auto Translation` to English via `Google Translation API`
  - `Display Names` or `Normal Names` Can be Used by Deafult *(Editable in Settings)*
  - `Custom Colors` or `Team Colors` Can be Used by Deafult *(Editable in Settings)*
- Type Searching for Console Logs
  - `type:server`, `type:client`, `type:error`, `type:warning`, `type:output`
  - `type:type searchString`
- Special Highlighting for Required Asset Logs
- Log History Restoration
  - `Right Click` the `Pause Button`
- Chat Log Quick Actions
  - `Left Click` a Log to Switch the Player's Name Between their `Display Name` and `Normal Name`
  - `Right Click` a Log to `Delete` it

## Server:
![Server](./Images/server.png)
- Player List
  - `Badges`, `Picture`, `Name`, `Display Name`, `User ID`, `Account Age`
- Server Info Display
  - `Name`, `Job ID`, `Uptime`
- Player Shortcuts
  - `Actions`, `Scan`, `Script Hub`

## Actions:
![Actions](./Images/actions.png)
- Player Info Display
  - `Badges`, `Picture`, `Name`, `Display Name`, `User ID`, `Account Age`
- Quick Command Actions
  - Tap on an `Action` to `Execute` it

## Scan:
![Scan](./Images/scan.png)
- Player Info Display
  - `Badges`, `Picture`, `Name`, `Display Name`, `User ID`, `Account Age`
- PlayerGUI Display
- Quick Item Actions
  - `Delete`, `Copy`, `Toggle`
- Copy All *(If Unique Item in List)*
- Local PlayerGui Support
  - Viewing Items that are Client Sided Only
  - Only Supported with the Local Player *(Not Other Players)*

##  Settings:
![Settings](./Images/settings.png)
- Features Section:
  - Auto Convert
  - Reset Mouse Icon
  - Ignore Invalid Targets
  - Log Client Console Logs
  - Command History
- Chat Logs
  - Translate
  - Translation Format
  - Use Display Names
  - Use Team Colors
- ESP
  - Toggle
  - Highlight
  - Display Titles
  - Use Team Colors
- Notifications
  - Toggle
  - Extra Command Notifications
  - Print to Console
  - Max Notifications
- Keybinds
  - High Priority Keybinds
  - Minimize
  - Command Bar
  - Inspect
  - ESP
- Closing
  - Close GUI
  - Hide GUI *(Hide the Phantom GUI for a Specified Amount of Time)*

## Inspect:
![Inspect](./Images/inspect.png)
- Inspect a Player to View Info About Them or Perform Actions
  - Hover the `Mouse` Over the Player's `Character`
  - Default Keybind: `F8`
- Player Info Display
  - `Badges`, `Picture`, `Name`, `Display Name`, `User ID`, `Account Age`
- Quick Actions
  - `Kill`, `Kick`, `Ban`, `More`
  - `More` will Open the `Actions` Page for the Following Player

## ESP:
![ESP](./Images/esp.png)
- Quickly See the Locaiton of Everyone in the Server
  - Default Keybind: `F6`
- Highlight Can be Enabled for Greater Visibility
- Name Titles Can be Toggled
- Custom Colors or Team Colors Can be Used

## Notifications:
![Notifications](./Images/notifications.png)
- Executor
  - Formatting Errors
  - Lua Errors
- Script Hub
  - Successfull Executions
  - Target Errors
  - Auto Conversion Errors
- Commands
  - Successes
  - Errors
- Logs
  - Required Asset Logged
  - Log Restoration
- Server
  - Owner Joined
  - Owner Left
  - Owner's Friend Joined
  - Owner's Friend Left
  - Player Hidden
  - Player Unhidden
- Settings
  - Invalid Hide Time

## Player Badges:
![Badges](./Images/badges.png)
- These Badges Can be Displayed in the Server, Actions, Scan, and Inspect Pages
- Purple: Local Player
- Red: Game Developer/Owner
- Blue: Game Developer/Owner Friend
- Orange: Hidden
- Yellow: Unhidden *(Was Previously Hidden)*

---

# Changelog

## [Version 1.9.2 (Latest)](https://github.com/FlowScript/Phantom/commit/453c355f0d5c8384ac87dbcfea96c6be2209d165)

**New Commands:**
- `Accessory`, `UnAccessory`
- `MeshAccessory`, `UnMeshAccessory`
- `Mesh`, `UnMesh`
- `Blur`, `UnBlur`
- `ColorCorrection`, `UnColorCorrection`
- `LocalBlur`, `UnLocalBlur`
- `LocalColorCorrection`, `UnLocalColorCorrection`
- `ScreenShake`, `UnScreenShake`
- `Face`, `UnFace`

### See the [CHANGELOG](./CHANGELOG.md) file for the full changelog.