# Athena - FNBR.co

Athena is a utility which generates the current Fortnite Item Shop into a stylized image and shares it on Twitter.

# Versions

[FortniteAPI.io](https://github.com/Liimiitz/Athena-FNAPI.io)

[Fortnite-API.com](https://github.com/Liimiitz/Athena-FNAPI.com)

[FNBR.co](https://github.com/Liimiitz/Athena-FNBR.co)

# Image Example

<p align="center">
    <img src="https://i.imgur.com/Ga7uWvd.jpg" width="650px" draggable="false">
</p>

## Requirements

- [Python 3.7](https://www.python.org/downloads/)
- [Requests](http://docs.python-requests.org/en/master/user/install/)
- [coloredlogs](https://pypi.org/project/coloredlogs/)
- [Pillow](https://pillow.readthedocs.io/en/stable/installation.html#basic-installation)
- [python-twitter](https://github.com/bear/python-twitter#installing)

A [FNBR.co API Key](https://fnbr.co/api/docs/) is required to obtain the Item Shop data, [Twitter API credentials](https://developer.twitter.com/en/apps) are required to Tweet the image.

## Usage

Open `configuration_example.json` in your preferred text editor, fill the configurable values. Once finished, save and rename the file to `configuration.json`.

- `delayStart`: Set to `0` to begin the process immediately
- `supportACreator`: Leave blank to omit the Support-A-Creator tag section of the Tweet
- `twitter`: Set `enabled` to `false` if you wish for `itemshop.png` to not be Tweeted

Edit the images found in `assets/images/` to your liking, avoid changing image dimensions for optimal results.

Athena is designed to be ran using a scheduler, such as [cron](https://en.wikipedia.org/wiki/Cron).

Start the bot by opening Command Prompt and entering the following command below.

```
python itemshop.py
```

## Credits

- Item Shop data provided by [FNBR.co](https://fnbr.co/)
- Original Creator: [EthanC](https://github.com/EthanC/Athena)
