This is a mirror of http://www.vim.org/scripts/script.php?script_id=1338

The plugin is derived from miniBufExplorer.
Only the modifiable buffer are displayed, and counted.
Key-bindings for buffer switching: <Alt-bufNumber>
Colored the tabs with the same color as StatusLineNC to create the impression
of tabs.

TabBar in winxp cmd:
http://photos1.blogger.com/blogger/4648/1229/1600/winxp_cmd.jpg

and gvim on winxp
http://photos1.blogger.com/blogger/4648/1229/1600/winxp.jpg


and gvim on linux+ion3
http://photos1.blogger.com/blogger/4648/1229/1600/screen.1.jpg

Known Supported Environments
----------------------------
- Windows:
    - GVim
- Linux:
    - GVim
    - Terminal (Gnome Terminal)
- Mac:
    - Terminal (iTerm)

Patched Functions
-----------------
1. Guess correct editing window after open/close/switch a buffer
2. Close buffer on the current buffer window ("Tbbd" command)
3. "E" command for more checking after open a buffer

Fixed Bugs
----------
1. The regular expression of close buffer matching is not good enough, so that  
if you want to close a "index.js" file while "index.js" and "..index.js" are open,  
it will cause endless function calls.

Mappings
--------
I add the following mapping for convenience in my *.vimrc*.

```vim
map bd <ESC>:Tbbd<CR>
map <C-n> <ESC>:Tbbn<CR>
map <C-p> <ESC>:Tbbp<CR>
```
