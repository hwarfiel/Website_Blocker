# Website_Blocker
F

### Description
fill in

## Author
Hayden Warfield

## Compatability

### installing locally:

1. save folder
2. go to `chrome://extensions`
3. toggle `Developer mode`
4. click `Load unpacked`
5. upload folder
6. extension should now be enabled!

### Sources

Based on this project: https://github.com/skinsshark/site-blocker

## Loopholes and Fixes

Extensions have an inherent loophole: you can always right-click the extension icon and hit "Remove from Browser". To prevent yourself from bypassing your own system when a distraction craving hits, modify your computer's OS Hosts File. This blocks the sites at the operating system root, applying to all present and future browsers automatically.

1. Open your terminal application (Terminal on Mac, or Command Prompt run as Administrator on Windows).

2. Open the host configuration:Windows: Type notepad c:\windows\system32\drivers\etc\hostsMac / Linux: Type sudo nano /etc/hosts

3. Scroll to the bottom and map the distraction domains to an unroutable IP (0.0.0.0):

```
0.0.0.0 facebook.com
0.0.0.0 ://facebook.com
0.0.0.0 instagram.com
0.0.0.0 ://instagram.com
```

4. Save and exit. The sites are now unreachable globally on your machine across every browser engine
