# A Colemak keymap for the Redox keyboard

----
![jeherve-redox-layout-2](https://user-images.githubusercontent.com/426388/44148042-ea49ac3a-a096-11e8-828e-8533fa75d569.jpg)

----

This keymap is **a work in progress**, and is meant to be used on Mac OS, with the "Unicode Hex Input" keyboard input.

![Mac OS keyboard input setting](https://user-images.githubusercontent.com/426388/43962498-1ee9e3fc-9cb8-11e8-88e3-dbb068ec5c67.png)

I may change a lot of the keys over the next few months, and will update this repo when I do so.

[View on KLE](http://www.keyboard-layout-editor.com/#/gists/3d5368842d87a8462c8f95d4382c4a19)

## Layers

My keymap uses 5 layers:

1. The default base layer, using [Colemak](https://colemak.com/).
2. A Symbol layer, so all symbols can be accessed from the home row. (top right legends)
3. A Navigation / Media layer, with both sound control and arrows on the home row. (bottom right legends)
4. An international / Emoji layer so I can type accented characters commonly used in France and in Hungary, as well as a few Emoji I often use. (top center legends)
5. A keyboard control layer, not pictured above, allowing me to control the LED lighting as well as the keyboard debug functions.

## Build

To use this keymap with your own Redox, you will need [the QMK firmware](https://github.com/qmk/qmk_firmware) checked out, and this repo either checked out to something like `keyboard/redox/keymaps/jeherve`, or symlinked there. One way to achieve that is this:

```
git clone https://github.com/qmk/qmk_firmware.git
cd qmk_firmware
git clone https://github.com/jeherve/redox-layout.git \ keyboard/redox/keymaps/jeherve
```

Once you've checked out the repo, you can build it like so:
```
make redox/rev1:jeherve
```

## Credits

- Redox keyboard design by [Mattia Dal Ben](https://github.com/mattdibi/redox-keyboard).
- This keymap is based off the default keymap for the Redox keyboard, available [here](https://github.com/qmk/qmk_firmware/tree/master/keyboards/redox) and also build by Mattia Dal Ben (thank you!).
- This layout uses [QMK keyboard controller firmware](https://github.com/qmk/qmk_firmware/).

I've also read posts by [Gergely Nagy](https://asylum.madhouse-project.org/blog/2016/10/15/multi-purpose-keys/), [Rebecca Le](https://sevenseacat.net/posts/2018/unicode-in-qmk-on-osx/), and [Justin Rogers](https://implementsblog.com/2016/10/16/my-ergodox-ezs-custom-layout/#comments) for inspiration.

## License

This keymap is licensed under GNU General Public License v2 (or later).
