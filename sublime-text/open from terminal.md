## mac:
``ln -s /Applications/Sublime\ Text.app/Contents/SharedSupport/bin/subl /usr/local/bin/subl``
## windows
### copy subl.exe. 
It is at sublime's installation folder: copy it in to a folder included in the system path. For example:

from C:\Program Files\Sublime Text 3

to C:\Windows\System32

### make a link
``mklink /h c:\windows\system32\subl.exe "c:\Program Files\Sublime Text 3\subl.exe"``
