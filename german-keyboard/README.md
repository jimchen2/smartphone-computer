German keyboard layout(qwerty and `;'[]` becomes `öäüß`):

1. Copy German Keyboard layout to `/usr/share/X11/xkb/symbols/tampered_de`
2. Add a new entry to `/usr/share/X11/xkb/rules/evdev.xml`

```
sudo sed -i "/<layoutList>/r tampered_de.layout.xml" /usr/share/X11/xkb/rules/evdev.xml
```

3. Clear the cache `rm -rf /var/lib/xkb/*`, log out and log in 
