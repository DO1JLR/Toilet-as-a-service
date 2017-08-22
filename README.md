# Toilet-as-a-service
info-beamer for raspberry pi with some videos you could know from the EH16 Toilet, from ZeTeCo or from Toolbox Bodensee e.V.

# Install Requirements:
You need to install the [Info-Beamer](https://info-beamer.com/pi) Version for the [Raspberry Pi](https://info-beamer.com/download/player) on your Raspberry Pi and Download some dependencies:

```bash
  sudo apt-get update
  sudo apt-get install ibevent-2.0-5 libavformat56 \
   libpng12-0 libfreetype6 libavresample2

```
*Maybe you have some [Trouble](https://raspberrypi.stackexchange.com/questions/59435/how-to-use-stretch-testing-packages) while istalling some deprecated packages...*


Follow [these](https://info-beamer.com/doc/info-beamer#raspberrypiversion) Instructions to prepare the ``/boot/config.txt`` file for the info-beamer like setting the option ``gpu_mem=192``.

## Update
Please Update the submodules in the git via:
```bash
  git submodule init && git submodule update

```

## Download Videos
Now Download some Videos you would like to play.
Or you can just Execute the Bash File do download some youtube Videos via youtube-dl and convert them in the correct size (1920x1080) if necessary.

But for this you need youtube-dl installed
```bash
  sudo apt-get install python3-pip ffmpeg youtube-dl
  ./download_videos.sh

```

