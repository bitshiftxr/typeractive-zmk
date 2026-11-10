# ZMK Corne Keyboard Layout

This this my personal [zmk](https://github.com/zmkfirmware/zmk) config for my
[corne keyboard](https://github.com/foostan/crkbd), the firmware is built to
work with the following devices.

- Keyboard: Typeractive Corne 6 column
- Controller: nice!nano v2 + nice!view (both halves)

> Standard split, no dongle. The left half is central and has ZMK Studio over USB.

## The Keyboard

![typeractive_kb](images/kb.jpeg)

> Nice!view shield is courtesy of
> [M165437's nice-view-gem](https://github.com/M165437/nice-view-gem).

## Keymaps

These are the keymaps and layers defined in this config. The keymaps were
generated using
[Nick Coutsos's Keymap Editor](https://nickcoutsos.github.io/keymap-editor/).

![keymaps](images/corne.svg)

**Macros**

- ⚡️ : hyper key (`ctrl` + `shift` + `alt` + `cmd`)
- ⚙️ : system settings (`cmd` + `shift` + `J`)
- 📷 : `printscreen` (linux) / `F13` (macos)
- `⌘⌥⎵` : homerow
- `⌃⎵` : tmux leader key
- `✦⎋`: `ctrl` + `shift` + `esc`
- adjust layer circle arrows: mouse movements
- adjust layer pan-arrows: scroll movements

> The image is generated using
> [Cem Aksoylar's Keymap-drawer](https://github.com/caksoylar/keymap-drawer)

## Installing Firmware

Run the **Build ZMK firmware** workflow, then download the artifact zip:

- nano_corne_left.uf2
- nano_corne_right.uf2
- nano_reset_settings.uf2

For each half (left first): plug it in, double-press reset, copy
`nano_reset_settings.uf2`. Double-press reset again and copy that half's
firmware. Then remove the old keyboard from Bluetooth settings and re-pair.
