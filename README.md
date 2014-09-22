# mp4towebm

Convert mp4 videos to webm.

### How to use

You need to specify a bitrate. For great quality, use `8M` as the first argument. For alright quality, use `2M` as the first argument. You can specify whatever you want. The higher the bitrate, the larger the filesize will be. All other arguments are treated as converting certain files only.

```bash
# Convert all files in current directory with 8M bitrate
mp4towebm 8M

# Convert certain files with 4M bitrate
mp4towebm 4M file.mp4 other_file.mp4 last_file.mp4

# Convert certain files with 3M bitrate
mp4towebm 3M new_*.mp4 to_process*.mp4

# Recursively convert all mp4 files with 8M bitrate
find . -type f -iname "*.mp4" -exec mp4towebm 8M '{}' \;
```
