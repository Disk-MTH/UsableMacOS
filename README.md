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

## [Maccy](https://github.com/p0deje/Maccy) - Clipboard Manager

### Install
`brew install --cask maccy`

### Config 
- Launch at login
- Open ^V (physical key Win+V)




AltTab


MOS


ScrollToZoom
