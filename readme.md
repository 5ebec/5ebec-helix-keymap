# The 5ebec's Helix Layout
## Layout

### Qwerty
```
,-----------------------------------------.             ,-----------------------------------------.
|   `  |   1  |   2  |   3  |   4  |   5  |             |   6  |   7  |   8  |   9  |   0  | Bksp |
|------+------+------+------+------+------|             |------+------+------+------+------+------|
| Tab  |   Q  |   W  |   E  |   R  |   T  |             |   Y  |   U  |   I  |   O  |   P  |  \   |
|------+------+------+------+------+------|             |------+------+------+------+------+------|
| Ctrl |   A  |   S  |   D  |   F  |   G  |             |   H  |   J  |   K  |   L  |   ;  |  '   |
|------+------+------+------+------+------+------+------+------+------+------+------+------+------|
| Shift|   Z  |   X  |   C  |   V  |   B  |   -  |   =  |   N  |   M  |   ,  |   .  |   /  |Enter |
|------+------+------+------+------+------+------+------+------+------+------+------+------+------|
|Adjust| GUI  | Alt  | Bksp | EISU |Space |   [  |   ]  |Space | KANA |Enter | Alt  | GUI  |Adjust|
`-------------------------------------------------------------------------------------------------'
```  

## Layers

|Priority|number|name|description|
| ---- | ---- | --- | --- |
|high|16|Adjust|Functions|
|low|0|Qwerty|QWERTY leyout(base)|

### Adjust 
```
,-----------------------------------------.             ,-----------------------------------------.
|  ESC |  F1  |  F2  |  F3  |  F4  |  F5  |             |  F6  |  F7  |  F8  |  F9  |  F10 |  Del |
|------+------+------+------+------+------|             |------+------+------+------+------+------|
|      |  F11 |  F12 |      |      |      |             |      |      |      |      |      |      |
|------+------+------+------+------+------|             |------+------+------+------+------+------|
|      |      | Vol- | Vol+ | Mute | Mac  |             | Left | Down |  Up  |Right |      |      |
|------+------+------+------+------+------+------+------+------+------+------+------+------+------|
|      |      |BrDown| BrUp |      | Win  |RGB ON| MODE | VAL- | VAL+ | HUE- | HUE+ | SAT- | SAT+ |
|------+------+------+------+------+------+------+------+------+------+------+------+------+------|
|      |      |      |      |      |      |      |      |      |      |      |      |      |      |
`-------------------------------------------------------------------------------------------------'
```

## Customize

see `rules.mk`

```
# Helix keyboard customize
# you can edit follows 7 Variables
#  jp: 以下の7つの変数を必要に応じて編集します。
HELIX_ROWS = 5              # Helix Rows is 4 or 5
OLED_ENABLE = no            # OLED_ENABLE
LOCAL_GLCDFONT = no         # use each keymaps "helixfont.h" insted of "common/glcdfont.c"
LED_BACK_ENABLE = no        # LED backlight (Enable WS2812 RGB underlight.)
LED_UNDERGLOW_ENABLE = no   # LED underglow (Enable WS2812 RGB underlight.)
LED_ANIMATIONS = yes        # LED animations
IOS_DEVICE_ENABLE = no      # connect to IOS device (iPad,iPhone)
```

## Compile

go to qmk top directory.
```
$ cd qmk_firmware
```

build
```
$ make helix:5ebec-helix-keymap
```

flash to keyboard
```
$ make helix:5ebec-helix-keymap:avrdude
```

## Link
* more detail wrote in Japanese [helix/Doc/firmware_jp.md](https://github.com/MakotoKurauchi/helix/blob/master/Doc/firmware_jp.md)
* [Helix top](https://github.com/MakotoKurauchi/helix)

