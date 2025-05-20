## Devices

- Computer: ThinkPad P16s (Fedora), Redmi Book (Windows)
- Smartphone: Redmi Note 13, Pixel Pro 8

## German keyboard

German keyboard layout(qwerty and `;'[]` becomes `öäüß`):

1. Copy German Keyboard layout to `/usr/share/X11/xkb/symbols/tampered_de`
2. Add a new entry to `/usr/share/X11/xkb/rules/evdev.xml`

```
sudo sed -i "/<layoutList>/r tampered_de.layout.xml" /usr/share/X11/xkb/rules/evdev.xml
```

3. Clear the cache `rm -rf /var/lib/xkb/*`, log out and log in

## Userscripts

- My Userscripts: [Video Sites Shortcuts Install](https://raw.githubusercontent.com/jimchen2/smartphone-computer/master/userscripts/video-sites-shortcuts.user.js) (Desktop Only), [YouTube Subtitles Install](https://raw.githubusercontent.com/jimchen2/smartphone-computer/master/userscripts/youtube-enhancer.user.js)
- Other Userscripts: [Voice Over Translation](https://raw.githubusercontent.com/ilyhalight/voice-over-translation/master/dist/vot.user.js)

## Communication

- Gmail
- Telegram(Russian)
- WhatsApp(German)
- WeChat
- [Website](https://jimchen.me)
