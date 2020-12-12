vim tips
========

tips for vim / nvim / ideavim / VSCodeVim

[:help object-motions](https://vimhelp.org/motion.txt.html#object-motions)

the basic:
----------


word
----
* dw - delete from cursor to next
* db - delete from cursor to previous
* diw - delete inside word
* `*` -
* `#` -
* `%` -

for html/jsx/xml/...
--------------------
* remember `*` `#` and `%` 
* `cat` - change a tag
* `cit` - change inner tag
* `dat` - delete a tag
* `dit` - delete inner tag
* `vat` - visual a tag
* `vit` - visual inner tag
* `vitp` - visual inner tag past
* `yat` - yank a tag
* `yit` - yank i tag

up/down
-------
* gg to first line
* G  to last line
* :10 to line 10
* 10G to line 10
* 10gg to line 10
* 50% to line 50% of file 


learn
-----
* :reg[isters]
* :marks
* :buffers :ls

tips
----

on linux, remape 'Caps Lock' key to 'Esc'
``` sh
setxkbmap -option caps:escape
```
