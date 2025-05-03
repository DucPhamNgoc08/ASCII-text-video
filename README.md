# ASCII Video Live

ASCII Video Live is a simple web app that converts your camera’s live video stream into real-time ASCII art. Each video frame is sampled pixel-by-pixel, converted to grayscale, and mapped to a character in a customizable density string.

## Features

* Live camera feed rendered as ASCII art in the browser
* Multiple density palettes for varying levels of detail and style
* Renders text inside a `<div>`, no `<canvas>` required
* Easy to customize and extend with your own character sets

### Live Previews

|                                           Preview 1                                           |                                           Preview 2                                           |                                           Preview 3                                           |
| :-------------------------------------------------------------------------------------------: | :-------------------------------------------------------------------------------------------: | :-------------------------------------------------------------------------------------------: |
| ![Preview 1](https://github.com/user-attachments/assets/d47213e8-327e-4dc8-86bc-86ca6d5eea37) | ![Preview 2](https://github.com/user-attachments/assets/4cdcb2c0-167e-4117-a310-0ccab5158f37) | ![Preview 3](https://github.com/user-attachments/assets/7a688d18-0dfd-4979-8df4-af3e872c7148) |

## Customizing the Density String

Open `sketch.js` and locate the `density` variable:

```js
// Example density options:
const density = "Ñ@#W$9876543210?!abc;:+=-,._          "; // Extended alphanumeric palette
const density = '       .:-i|=+%O#@';               // Bourke’s short grayscale ramp
const density = '        .:░▒▓█';                        // Unicode block shading ramp
```

* Replace the string assigned to `density` to map brightness to your own ASCII characters.
* More characters = more grayscale levels = smoother art.

## License

This project is licensed under the [MIT License](LICENSE).
