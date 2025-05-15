# `debugfile.inc`

A RGBDS macro pack to ease working with debugfiles: zero-cost runtime assertions, now for your GB game!

A manual of sorts is available [on **the wiki**](http://github.com/ISSOtm/debugfile.inc/wiki).

## Why `debugfile.inc`

These macros let you make the emulator check that your assumptions hold, even at runtime; and even better, this is done without modifying the ROM.
This means no `jr`s becoming out of range from long debug strings, or other unpleasant surprises.

You can check for things as simple as “the B register shouldn't be zero here”, as convenient as “did the stack overflow?”, and as complex as “this 16-bit variable should point just before a byte with bit 4 set”.

## Debugfile support

Currently, [Emulicious] is the only GB emulator supporting debugfiles.

[Emulicious]: https://emulicious.net
