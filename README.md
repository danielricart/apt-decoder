# NOAA APT Decoder

Decode analog, APT signals from the NOAA weather satellites.

## Requirements

- python 2
-- not tested in Python 3
- pip
-- open a terminal console and type `pip` . 
-- If you get an error, install `pip`:

    sudo easy_install pip

## Setup

    pip install -r requirements.txt

## Usage
### Downsampling

If your file is not at the correct sampling rate, resample it:

    python resample.py soundfile.wav
    
You will obtain a file called `resampled.wav` that you can use for decoding instead of the original `soundfile.wav`

### Decoding

    python apt.py soundfile.wav image_out.png

## Examples

![Example image](./examples/example.png)

## Alternatives

You can also try [wxtoimg](http://wxtoimg.com/) but looks dead.

Alternatively [atp-dec/apt-dec](https://github.com/csete/aptdec) works really
good. Keep in mind that the [1.7
release](https://github.com/csete/aptdec/releases) looks newer than the [repo's
master branch](https://github.com/csete/aptdec).
