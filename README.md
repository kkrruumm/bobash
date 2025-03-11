# bobash
A simple [bobashare](https://github.com/BBaoVanC/bobashare) client written in bash.

# Usage

```
bobash upload file - Uploads file to the specified bobashare server.

bobash delete id deletekey - Deletes ID on the specified bobashare server.

bobash log - Outputs contents of the log file.
```

All uploads and their details (such as IDs and delete keys) will be logged in, by default, ``~/.local/share/bobash/log``.

A few settings may be changed in ``~/.config/bobash/config``, 

```
server - Set the API url for the target bobashare server.
logdir - Set the logging directory for bobash uploads.
stripping - Enable or disable exif data stripping from uploads, depends on exiftool. Valid values are true or false, defaults to false.
```

# Dependencies
* exiftool (Optional, for exif data stripping)
* printf
* curl
* file
* jq
* cat
