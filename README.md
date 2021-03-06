![Image](https://farm1.staticflickr.com/580/33704162375_e0883536cf_o.png)

# NightPatch

Enable Night Shift on any old Mac models.

You have to disable SIP (System Integrity Protection) before applying. [How to disable SIP](http://apple.stackexchange.com/questions/208478/how-do-i-disable-system-integrity-protection-sip-aka-rootless-on-os-x-10-11)

Backup your Mac before applying.

Not compatible with some third-party monitors.

Referenced [Pike's blog](https://pikeralpha.wordpress.com/2017/01/30/4398/).

## Supported macOS build

- macOS 10.12.4 (16E195)

- macOS 10.12.5 Developer Preview 1 (16F43c)

- macOS 10.12.5 Public Beta 1 (16F43c)

## How to patch

`$ cd /tmp; curl -o NightPatch.zip https://codeload.github.com/pookjw/NightPatch/zip/master; unzip NightPatch.zip; cd NightPatch-master; ./NightPatch.sh`

## How to revert

`$ cd /tmp; curl -o NightPatch.zip https://codeload.github.com/pookjw/NightPatch/zip/master; unzip NightPatch.zip; cd NightPatch-master; ./NightPatch.sh -revert`

## Troubleshooting

- patch/patch-BUILD is missing.

: That’s because I didn’t make a patch file for your macOS. I’ll make for you when it possible.

- ERROR : Turn off System Integrity Protection before doing this. / ERROR : Can't write a file to root.

: [Solution](http://apple.stackexchange.com/questions/208478/how-do-i-disable-system-integrity-protection-sip-aka-rootless-on-os-x-10-11)
