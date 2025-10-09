# UsableMacOS
Make a Mac nearly usable for a Windows user

For everything you will need Homebrew
Every config is a personnal preference, you can change it

Apps:

## [Karabiner-Elements](https://github.com/pqrs-org/Karabiner-Elements) - Keyboard remapper

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

## [MOS](https://github.com/Caldis/Mos) - Mouse fine-tuning

### Install
`brew install --cask mos`

### Config
Under "General"
- Smooth Scrolling
- Reverse Scroll
- Launch on Login
- Hide Status Bar Icon

## [Scroll To Zoom](https://github.com/alphaArgon/ScrollToZoom) (1,0.5) - In-app zoom and not OS zoom

### Install
Get the [latest realease](https://github.com/alphaArgon/ScrollToZoom/releases), unzip it and put it in your "Applications" folder

### Config
- Use Scroll gesture to zoom with ⌘ (physical key: Ctrl)
- Fingers up to zoom in
- Allow Mgic Mouse gestures
- Launch Scroll To Zoom at login

## [AltTab](https://github.com/lwouis/alt-tab-macos) - Alt+Tab by window (an not by app)

### Install
`brew install --cask alt-tab`

### Config
Under "General"
- Start at login

Under "Controls"
- Trigger shortcut: Hold ⌥ and press ⇥ (physical keys: Alt+Tab)
- After release: Focus selected window
- Show windows from Spaces: All apps
- Show windows from screens: All screens
- Show minimized windows: Show
- Show hidden windows: Show
- Show fullscreen windows: Show
- Show apps with no open window: Hide
- Order windows by: Recently Focused First

Under "Appearance"
- Show on: Screen including mouse

## [Maccy](https://github.com/p0deje/Maccy) - Clipboard Manager

### Install
`brew install --cask maccy`

### Config 
- Launch at login
- Open ⌃V (physical keys: Win+V)




AltTab


MOS


ScrollToZoom
