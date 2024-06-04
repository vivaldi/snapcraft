# vivaldi-snapcraft

This repository contains packaging files for snap packaging for vivaldi

## Building

To package this, simply run snapcraft while being in the directory containing these files.

## Running

Currently, when packaging locally, there are two connections needed to be done by hand to make the browser work as intended:

### Sandboxing

```
snap connect vivaldi:browser-sandbox
```

### FFMPEG (Proprietary codecs)

```
snap connect vivaldi:chromium-ffmpeg-115016 chromium-ffmpeg:chromium-ffmpeg-115016
```

These will have to be requested to be auto-connected in snap store (TODO right here, eh?!)