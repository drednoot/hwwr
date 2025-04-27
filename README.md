# History Wrapper (ythw)

A simple wrapper around mpv and yt-dlp to add history functionality to it

# Requirements
 - yt-dlp
 - jq

# Usage
```
ythw [-hb] [link]
  -h    show this help
  -b    browse history
```

Type `ythw` to play latest video or `ythw -b` to browse history and select a video from there.
You can also add videos by typing `ythw <link>`.

# Installation

Run the install script:
```
sudo ./install.sh
```

This will install the script to `/usr/local/bin/ythw`

# Uninstall

Run the uninstall script:
```
sudo ./uninstall.sh
```

This will remove the script from `/usr/local/bin/ythw`

# Other notes

## History file

History file is contained in your `$HOME/.config/ythw/history.json`, the spec for the json could be found in [spec](spec.norg) file.

## Environment variables
 - `CONFIG_FILE` - path to the history.json, default: `$HOME/.config/ythw/history.json`
 - `PLAYER` - path to your video player, default is `mpv`
 - `YTDL` - path to your yt-dlp, default is `yt-dlp`
 - `HISTORY_DISPLAY_SIZE` - number of history items to display, default is `10`

# License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
