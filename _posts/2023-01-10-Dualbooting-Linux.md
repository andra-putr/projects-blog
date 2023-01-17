---
published: true
---
## Intro

Started with Ubuntu dualbooting Win 10, but corrupted for some reason.
Decided might as well try Kali linux since I wanted to play around with pentesting stuff, so that's what I'm using now.

Still lost few things along the way though like my custom login screen based around Lain's Copland OS thing I found on github.

# Keyboard Bindings
Had to use different binds since each of them couldn't do the other for some reason, at least it works for the most part.

Current settings: 
- Caps lock & CTRL swap = [XKB file edit](https://gist.github.com/dmgl/f5ec96dfe3af1652792089ebf6683431)
- Backspace and Backslash swap = [xmodmap commands + autostart on boot](https://askubuntu.com/questions/54157/how-do-i-set-xmodmap-on-login)
- ~~IJKL Arrow keys (Alt+IJKL for arrow keys)~~ = [Autokey](https://github.com/autokey/autokey)
	- **UPDATE**: As of 2023/1/16, due to me wanting to learn vim I've changed it to HJKL instead.

## Japanese Input

This was initially quite an annoying issue to deal with for me, since I was really adamant about my keyboard shortcuts (as can be seen with me having all those keyboard macros and switches). Since inputting Japanese through a keyboard requires you to press several more keys to choose input method etc., this also of course meant that my usual workflow when using Japanese on a computer is also modified quite a bit and I am really only fully comfortable with my own setup. 

### JP Input on Windows
I first learned Japanese (including how to type in Japanese) on a windows machine back home, so it naturally became the input method that I'm most used to. I used Google's Japanese IME on a standard ANSI keyboard which had shortcuts such as:
- Win + Spacebar = Switch language (Windows shortcut)
- L_Alt + \` = Switch input mode (Romaji --> 仮名)
- Shift + Caps_Lock = Switch Kana input mode (ひらがな　--> カタカナ)

There were more I believe, such as F7 or something to convert selected text into katakana, double/half width conversion, etc. But I never really used them much and mostly relied on the above mentioned shortcuts. My goal then was to of course try and find a way to have the same shortcuts set up on my Linux machines.

### JP Input on Linux
![enter image description here](https://imgur.com/fI5u2ORl.png)
I really thought importing my settings from Windows would be much easier than it was, but alas quite a bit of tinkering was needed. When I was still using Ubuntu, I had a solution that kind of worked? But I never really liked it since it had issues like:

- Couldn't use Windows key and \` key for some reason as shortcuts???
- Was stuck on JIS layout, could not easily find option to switch to ANSI with Japanese input

Which meant that:
- I had to use mouse manually to switch between EN and JP
- I had to use mouse manually to switch between Romaji and kana input
- I had to use mouse manually to switch between hiragana and katakana
- I had to blindly find where symbols are located under since JIS layout places them in different locations VS ANSI

![JIS Thinkpad keyboard](https://i.stack.imgur.com/t592d.jpg)

Which made me HATE using it. I ended up having to always switch back to my Windows partition whenever I go to Japanese class. 

I'm sure you're already saying to yourself 

# Mouse Stuff
Mostly pretty good, was just annoyed that Kali doesn't have an easy way to disable the "Middle mouse to paste" thing that Linux for some reason has. With Ubuntu GNOME it was easy enough to run `gnome-tweaks`, but since my Kali was on XFCE I wasn't sure on how to do that.

After a bit of searching I ended up following [this thread](https://unix.stackexchange.com/questions/24330/how-can-i-turn-off-middle-mouse-button-paste-functionality-in-all-programs) I found from reddit. I made the file and set it to launch on startup, bob's your uncle mary's your aunt it works well.
# Future Things

- Method to export/import keyboard bindings etc. easily between all my Linux machines
	- Export as package or something maybe?
- Mouse/Trackpad
	- Still unhappy about lack of features l
- Fingerprint scanner
	- Maybe drivers required? Not sure if lenovo provides for Linux
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTE1MzI5NjMyNzYsMjIwNDQ5MTI0LDEyNT
A1NzYxNywxNjczODE4MDcwLC0xNTg3Njg0NjEzXX0=
-->