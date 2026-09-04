# Arduino Snake Game Project

A compact Snake game for Arduino that renders gameplay on an 8×8 MAX7219 LED matrix. Four push-buttons control movement, and four indicator LEDs provide directional feedback.

## Features

- Wrap-around 8×8 game board
- Random apple placement
- Snake growth and self-collision reset
- Debounced directional input

## Hardware

- Arduino Uno or compatible board
- MAX7219 8×8 LED matrix
- 4 momentary push-buttons
- 4 LEDs with suitable current-limiting resistors

## Wiring

| Function | Arduino pin |
| --- | --- |
| Matrix DIN | 12 |
| Matrix CS | 11 |
| Matrix CLK | 13 |
| Up / Down / Left / Right buttons | 2 / 3 / 4 / 5 |
| Direction LEDs | 7 / 8 / 9 / 10 |

Buttons use `INPUT_PULLUP`; wire each button between its pin and GND.

## Setup

1. Install the **LedControl** library in the Arduino IDE.
2. Open `Source Code` (rename it to `SnakeGame.ino` if your IDE requires an `.ino` extension).
3. Wire the hardware as listed above and upload.

## Project files

- `Source Code` — Arduino sketch
- `image.jpg` — project image
- `document_SG.docx` — supporting project document

## Improvement ideas

- Add a score display or sound feedback.
- Replace blocking `delay()` calls with a `millis()`-based game loop.
- Add a start/game-over screen and difficulty levels.

## License

No license has been specified. Add one before reusing or distributing this work.