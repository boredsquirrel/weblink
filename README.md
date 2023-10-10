# weblink
A small bash tool to create GUI desktop links for websites including favicon and .desktop entry

Some people like to launch Websites either from their Appmenu, or from their Desktop.
Even though thats rather weird, it can't harm to help with that!

The tool:
- uses core GNU utils, so it should work everywhere (except Alpine, lol)
- detects if the user uses native for Flatpak firefox
- downloads the matching favicon using the DuckDuckGo favicon search
- Extracts the websites Titles
- Removes Umlauts from the Title
- Creates a Desktop entry with all the parameters, using any given URL

Install:
```
mkdir -p ~/.local/share/applications/DESKTOP-LINKS
mkdir ~/.local/share/applications/DESKTOP-LINKS-ICONS

wget -P ~/.local/bin/ https://github.com/trytomakeyouprivate/weblink/raw/main/weblink
chmod +x ~/.local/bin/weblink
```

Use:
```
weblink wikipedia.org
```

TODO:
- create a Firefox Addon to do this for the currently visited website
- fix all special characters, not only Umlauts
