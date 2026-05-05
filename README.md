# ircII UTF-8 patches

Patches against ircII 20260115 adding UTF-8 handling to input and window code. Suitable only with 1 or 2 byte chars.
set IRC_ENCODING UTF-8
set INPUT_ENCODING UTF-8
set DISPLAY_ENCODING UTF-8
set EIGHT_BIT_CHARACTERS ON


## Apply

Place both patch files in the root of the ircII source tree, then:

    cd ircii-20260115
    patch -p0 < utf8_input.patch
    patch -p0 < utf8_window.patch

This patches `source/input.c` and `source/window.c`.

## Files

- `utf8_input.patch` – UTF-8 aware input line editing
- `utf8_window.patch` – UTF-8 aware window/display rendering

## License

Same terms as upstream ircII.
