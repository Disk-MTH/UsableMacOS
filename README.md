# UsableMacOS
Make a Mac nearly usable for a Windows user

## Introduction

For the majority of the installations, you will need [Homebrew](https://docs.brew.sh/) installed on you Mac

You will have to grant premissions to each app for various things, juste read what they are asking for, evrything is written

Every configuration I provide below are personnal preferences, you are free to change it

Each of the config lines are the changes I made from the default setup, or important things to change if your default config is not the same anymore

## [Karabiner-Elements](https://github.com/pqrs-org/Karabiner-Elements) (15.5.0) - Keyboard remapper

### Install
`brew install --cask karabiner-elements`

### Config
Under "Devices"
- Disable "Modify events" for all native devices (like internal keyboard and trackpad for a MacBook)
- Enable "Modify Events" and "Ignore vendor events" for your Windows devices (keyboard and mouse) 

Under "Complex modifications" use "Add your own Rule" for each
- Spotlight on Win
- Finder on Win+E
- Settings on Win+I
- Lock on Win+L
- Menu bar on Ctrl+ClickR (will be effective after the "meuanywhere" step)
- Terminal on F4 (will replace spotlight on F4)
- Swap Cmd and Ctrl
- Swap Ctrl and Alt for Arrows
  - Arrow move to previous/next char
  - Ctrl+Arrow move to previous/next word
  - Alt+Arrow move start/end of line
  - Shift modifier make previous modifiers do a selection
- Swap Ctrl and Alt for Backspace
  - Backspace delete a char
  - Ctrl+Backspace delete a word
  - Alt+Backspace delete the line

After that your bindings will be effective. For the rest of the process, you have to remember that the logical key you will see in softwares may not correspond to the physical key you pressed

## [MOS](https://github.com/Caldis/Mos) (3.5.0) - Mouse fine-tuning

### Install
`brew install --cask mos`

### Config
Under "General"
- Smooth Scrolling
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
```
brew tap acsandmann/tap
brew install menuanywhere
```

### Config
- Create the config file: `mkdir -p ~/.config/menuanywhere && [ ! -f ~/.config/menuanywhere/config.json ] && touch ~/.config/menuanywhere/config.json`
- Copy the config inside

After that you need to restart the Mac for the config to be effective

## [Maccy](https://github.com/p0deje/Maccy) (2.5.1) - Clipboard Manager

### Install
`brew install --cask maccy`

### Config 
Under "General"
- Launch at login
- Open ⌃V (physical keys: Win+V)
- Paste automatically


