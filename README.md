## ThorsHammer

GBTH client for modern platforms



https://github.com/user-attachments/assets/be3c46ca-a678-4b73-885f-bfdec8f87345



### Features

- Should just work on modern Windows, without additional compatibilty modes / DxWnd
- UTF8 engine
- Natively uses 32-bit graphics (but imperceptible since the assets are 16-bit anyway)
- Doesn't require a launcher, but still supports oldschool launchers
- Windowed by default, enter windowed-fullscreen via Alt+Enter
- Data files in CSV
- No administrator rights required, runs happily as a regular user
- Screenshots in PNG
- IME _sometimes_ works
- Behaves mostly like a late-TH client

### Caveats

- Free, but not open-source
- Does not run in Wine/Proton/Crossover
- Buddy components are largely unimplemented/broken
- AV/EDRs might flag the main executable file, might require adding an exception
- Published as-is, I don't know what I'm doing, I am unable to offer support or feature requests


### Network Protocol

A reference server is not available yet, but it should be mostly compatible with late-TH (e.g. EXItem/PU) servers. While untested with this client, Luiz's [GunBound-Java](https://github.com/kyll3r/GunBound-Java) looks like a promising candidate to start from. Bear in mind that all strings must be encoded in UTF8.


### Setup

Download/clone, edit `SystemPreferences.ini` with your server's address, then run the client. No installation is required, and this client does not store preferences in the registry.


### Login

Credentials can be supplied through three different ways:

- GME style, 96-byte createprocess "oldschool" style
- Command line, `client.exe username password`, easier to work with, doesn't support spaces
- Internal UI, if neither of the prior parameters are present, a login screen is shown during startup


### Anticheat

None. Regular anticheats are ineffective here, in the same way where process-level/kernel anticheats don't work on chess/sudoku, since trajectory planning can be trivially solved via e.g. pixel bots. For this reason, this client is fine running as a limited user. A stronger emphasis on trust-based strategies (e.g. invitation trees, reputation, active moderation) will probably work better.


### Source

The binaries are released for free, however it is not accompanied by its source. I resent the idea that this client may be used for commercial gain, as it goes against the spirit of preserving this two-decade old game.

The client is lightly packed/protected, the idea being that it will take less effort to figure out GBTH behavior by simply looking at an unpacked GBTH client (e.g. GBS404, includes logging!) instead of this.


### Github

Github is selected as a distribution platform and also as a space for discussion and issue tracking. If there's a better alternative, I'll be happy to take a look. Use the "incognito" litmus test for whether a platform is valid - if any attachments, links, files, images, messages are intentionally made unavailable to a guest (e.g. discord, rage zone), then it is not a suitable platform.


## Thanks

- Original gang: kasi (까시), comsik (녹염), cozy, enddream, yesoori, oorusa, jaeyong, yaong2, jchlee75, reddragon, designer, johnny5, loserii, scjang, chuko, pirania, blash45, knights, cosmos, ethera,  (now with UTF-8, Cosmos' credits is more accessible, via `/코스모스`)
- .BE: phnx, kimmy
