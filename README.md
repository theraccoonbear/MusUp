# MusUp

Get that album ready for a YouTube upload

This Perl script depends on `id3tool` and `ffmpeg` that are invoked through the shell but is otherwise vanilla.

## Usage:

```
$ ./musup <path-to-album>
```

## Notes:
* Expects and only works with .mp3 files (files are simply cat'ed together)
* Expects a file called cover.jpg in the same directory as the mp3s
* Will read ID3 tags from files
* Will read track lengths from files
* Generates an album-upload.mkv in /output using the cover art as the "video" and all of the cat'ed tracks as the audio
* Generates an album-description.txt in /output containing numbered track list with linkable timestamps

## To Do:
* Include album/artist/year in description
* Add config
* Upload to YouTube directly