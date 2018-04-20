# Video Thumbnail Generator
Generate thumbnail sprites from videos and create preview video from thumbnails

## Build

1. Clone it:

```sh
$ git clone git@gitlab.cbg:cbg/videoThumbnailGenerator.git
```

2. Then go to the project's folder:

```sh
$ cd videoThumbnailGenerator
```

3. And finally run:
```shell
$ chmod a+x build && ./build
```

## Run
```shell
$ ./generator --help
Video Thumbnail Generator

Usage:
  ./generator <video> <width> <height> <columns> <output> <video_preview>
  ./generator (-h | --help)
  ./generator --version

Options:
  -h --help         Show this screen.
  --version         Show version.
  <video>           Video file path.
  <width>           Width of each index.
  <height>          Height of each index.
  <columns>         Total number of thumbnails per line.
  <output>          Output.
  <video_preview>   Preview video path.
```

## Example
```shell
$ ./generator showtv.mp4 163 88 10 thumbnails/43534.jpg previews/43534.mp4
Extracting 10 frames
  [####################################]  100%
Frames extracted.
[MoviePy] >>>> Building video previews/43534.mp4
[MoviePy] Writing video previews/43534.mp4
100%|███████████████████████████████████████| 121/121 [00:00<00:00, 2146.97it/s]
[MoviePy] Done.
[MoviePy] >>>> Video ready: previews/43534.mp4 

Saved!
```
