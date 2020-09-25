## Forked from yueyoum/vim-linemovement
This fork delete ctrl+o map.

```
diff --git a/plugin/linemovement.vim b/plugin/linemovement.vim
old mode 100644
new mode 100755
index 7dae096..073c71e
--- a/plugin/linemovement.vim
+++ b/plugin/linemovement.vim
@@ -50,10 +50,3 @@ if !exists("g:linemovent_mapped_keys")
 
     let g:linemovent_mapped_keys = 1
 endif
-
-
-" Add empty line of above and bellow of one line
-noremap <silent> <c-o> O<ESC>jo<ESC>k
-
-
-
```

# linemovement.vim

Simplify the line movement in vim


## install

Using [vundle](https://github.com/gmarik/vundle)
or [pathogen](https://github.com/tpope/vim-pathogen)

    vundle example:

    " add the following line in your .vimrc
    Bundle 'yueyoum/vim-linemovement'

    " save it and run BundleInstall


## Key bindings

`ctrl-Up` moving up    *(Up is up arrow key)*

`ctrl-Down` moving down   *(down is down arrow key)*

`ctrl-shift-o` adding empty lines at the above and bellow of current line.
**just work in normal mode**


#### Custom

You can change the default key bindings.

Add the following line in your `.vimrc`

    let g:linemovement_up="<c-Up>"
    let g:linemovement_down="<c-Down>"


replace the key bindings whatever you want!


##### move one line or block in any mode.

![moving_line](http://i1297.photobucket.com/albums/ag23/yueyoum/line1_zps05d31091.gif)

##### expand margin spaces, adding empty lines above and bellow the line.

![expand_line](http://i1297.photobucket.com/albums/ag23/yueyoum/line2_zpsfd213adc.gif)

