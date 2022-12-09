---
layout: post
title: Thinkpad X1 Carbon 5th Gen Revamp for 2022.html
date: 2022-12-8
published: true
---
Restoring laptop for 2022 > Buying new laptop

## Intro

Been a while since I've had this thing, bought it all the way back in 2017 when I was getting ready to go to uni in Melbourne.
Was gonna take computer science, so was thinking a thinkpad would be fitting for that role.
Here are some of the things I want to do to it:

- Hardware
  - New battery
  - New SSD
  - Replace thermal paste
- Software
  - Dualboot Ubuntu
  - GNU GRUB Themes
  - Custom boot logo
  - Ubuntu issues
      - Trackpad gestures
      - Fingerprint scanner
      - Re-making macros (arrow keys layer, CTRL CAPS swap, etc.)
      - Japanese IME with ANSI keyboard


## Hardware
### New Battery
After about 5 years of use, the battery went down from its original capacity of 57MwH --> ~21MwH.
This meant that the battery life went from about 7+ hours to barely 2 hours! Surprised I didn't even realize how bad it was, I suppose the change was too gradual for me to notice until I ran a 
> powercfg /batteryreport

![](https://i.imgur.com/V0m0Pr7.png)

After some time searching for a replacement (and after dodging a shady site in Japan), my battery arrived from Amazon in about 3 days time.

Replacement was fairly straight forward, really makes me glad I own a thinkpad where I can do things like this without a heat gun. After replacement the battery now registers back to 57MwH and lasts up to 8+ hours again!

![](https://i.imgur.com/rpFwipd.png)

To make sure it lasts longer however, I followed [this guide](https://www.ultrabookreview.com/31385-the-throttlestop-guide/) to set up Throttlestop on my laptop. 
Hopefully this makes it last longer, though I don't know for sure since the increase I got from replacing the battery eclipses any gains Throttlestop might have given.


### New SSD

### New Thermal Paste
