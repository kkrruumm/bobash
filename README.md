# bobash
A simple [bobashare](https://github.com/BBaoVanC/bobashare) client written in bash.

# Usage

```
bobash upload file - Uploads file to the specified bobashare server.

bobash delete -i <id> -k <deletekey> - Deletes ID on the specified bobashare server.

bobash log - Outputs contents of the log file.

On uploads exiftool cannot strip, assuming stripping is enabled, you may add the --keep-exif flag to disable exif stripping on a per-upload basis.
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
* bash
* echo 
* curl
* file
* jq
* cat
