# bobash
A simple bobashare client written in bash.

# Usage

```
bobash upload file - Uploads file to the specified bobashare server.

bobash delete id deletekey - Deletes ID on the specified bobashare server.

bobash log - Outputs contents of the log file.
```

All uploads and their details (such as IDs and delete keys) will be logged in, by default, ``~/.local/share/bobash/log``.

You may change the bobashare server this points at or the log directory location by editing ``~/.config/bobash/config``.

# Dependencies
* printf
* curl
* file
* jq
* cat
