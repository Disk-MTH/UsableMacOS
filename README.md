# UsableMacOS
Make a Mac nearly usable for a Windows user

## Introduction

For most installations, you will need [Homebrew](https://docs.brew.sh/) installed on your Mac.  

You will have to grant permissions to each app for various features. Just read what they are asking for — everything is explained.

Some of the app may be blocked by MacOS, you need to allow them in "Privacy & Security" settings

Every configuration I provide below reflects my personal preferences; you are free to change them.  

Each configuration line represents changes I made from the default setup or important adjustments if your default configuration differs.  

## [Karabiner-Elements](https://github.com/pqrs-org/Karabiner-Elements) (15.5.0) - Keyboard remapper

### Install
`brew install --cask karabiner-elements`

### Config
Under "Devices"
- Disable "Modify events" for all native devices (like internal keyboard and trackpad for a MacBook)
- Enable "Modify Events" and "Ignore vendor events" for your Windows devices (keyboard and mouse) 

Under "Complex modifications" use "Add your own Rule" for each
- [Spotlight on Win](https://github.com/Disk-MTH/UsableMacOS/blob/main/karabiner-elements/Spotlight%20on%20Win.json)
- [Finder on Win+E](https://github.com/Disk-MTH/UsableMacOS/blob/main/karabiner-elements/Finder%20on%20Win%2BE.json)
- [Settings on Win+I](https://github.com/Disk-MTH/UsableMacOS/blob/main/karabiner-elements/Settings%20on%20Win%2BI.json)
- [Lock on Win+L](https://github.com/Disk-MTH/UsableMacOS/blob/main/karabiner-elements/Lock%20on%20Win%2BL.json)
- [Emojis on Win+Space](https://github.com/Disk-MTH/UsableMacOS/blob/main/karabiner-elements/Emojis%20on%20Win%2BSpace)
- [Menu bar on Ctrl+ClickR](https://github.com/Disk-MTH/UsableMacOS/blob/main/karabiner-elements/Menu%20bar%20on%20Ctrl%2BClickR.json) (will be effective after the "meuanywhere" step)
- [Terminal on F4](https://github.com/Disk-MTH/UsableMacOS/blob/main/karabiner-elements/Terminal%20on%20F4.json) (will replace spotlight on F4)
- [Swap Cmd and Ctrl](https://github.com/Disk-MTH/UsableMacOS/blob/main/karabiner-elements/Swap%20Cmd%20and%20Ctrl.json)
- [Swap Ctrl and Alt for Arrows](https://github.com/Disk-MTH/UsableMacOS/blob/main/karabiner-elements/Swap%20Ctrl%20and%20Alt%20for%20Arrows.json)
  - Arrow move to previous/next char
  - Ctrl+Arrow move to previous/next word
  - Alt+Arrow move start/end of line
  - Shift modifier make previous modifiers do a selection
- [Swap Ctrl and Alt for Backspace](https://github.com/Disk-MTH/UsableMacOS/blob/main/karabiner-elements/Swap%20Ctrl%20and%20Alt%20for%20Backspace.json)
  - Backspace delete a char
  - Ctrl+Backspace delete a word
  - Alt+Backspace delete the line

**The order of modifications matter, respect it**
After this, your key bindings will be active. Keep in mind that the logical key shown in software may not match the physical key you pressed.  

## [MOS](https://github.com/Caldis/Mos) (3.5.0) - Mouse fine-tuning

### Install
`brew install --cask mos`

### Config
Under "General"
- Reverse Scroll
- Launch on Login
- Hide Status Bar Icon

## [Scroll To Zoom](https://github.com/alphaArgon/ScrollToZoom) (1.0.5) - In-app zoom (and not OS zoom)

### Install
Get the [latest realease](https://github.com/alphaArgon/ScrollToZoom/releases), unzip it and put it in your "Applications" folder

### Config
- Use Scroll gesture to zoom with ⌘ (physical key: Ctrl)
- Fingers up to zoom in
- Allow Mgic Mouse gestures
- Launch Scroll To Zoom at login

## [AltTab](https://github.com/lwouis/alt-tab-macos) (7.30.0) - Alt+Tab by window (and not by app)

### Install
`brew install --cask alt-tab`

### Config
Under "General"
- Start at login

Under "Controls"
- Trigger shortcut: Hold ⌥ and press ⇥ (physical keys: Alt+Tab)
- Show apps with no open window: Hide

Under "Appearance"
- Show on: Screen including mouse

## [MenuAnywhere](https://github.com/acsandmann/menuanywhere) (1.0.6) - Make the top menu bar avaiblable anywhere

### Install
**You need XCode installed on your Mac.**

```
brew tap acsandmann/tap
brew install menuanywhere
```

### Config
- Create the config file: `mkdir -p ~/.config/menuanywhere && [ ! -f ~/.config/menuanywhere/config.json ] && touch ~/.config/menuanywhere/config.json`
- Copy the [config](https://github.com/Disk-MTH/UsableMacOS/blob/main/menuanywhere/config.json) inside

Restart your Mac for the configuration to take effect.  

## [Maccy](https://github.com/p0deje/Maccy) (2.5.1) - Clipboard Manager

### Install
`brew install --cask maccy`

### Config 
Under "General"
- Launch at login
- Open ⌃V (physical keys: Win+V)
- Paste automatically


