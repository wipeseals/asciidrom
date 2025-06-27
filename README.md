# Asciidrom

[![Deploy static content to Pages](https://github.com/wipeseals/asciidrom/actions/workflows/deploy.yml/badge.svg)](https://github.com/wipeseals/asciidrom/actions/workflows/deploy.yml)

A web-based tool that converts [WaveDrom](https://wavedrom.com/) timing diagrams to ASCII art, making it easy to include waveforms in source code, documentation, and text-based formats.

🔗 **Live Demo:** [https://wipeseals.github.io/asciidrom/](https://wipeseals.github.io/asciidrom/)

## Overview

Asciidrom bridges the gap between visual timing diagrams and text-based documentation. It takes WaveDrom JSON input and converts it into clean ASCII art that can be easily copied and pasted into source code comments, README files, or any text-based medium.

## Features

- **WaveDrom to ASCII Conversion**: Convert WaveDrom JSON timing diagrams to source-code-friendly ASCII art
- **Real-time Preview**: See your ASCII output update as you type
- **Dark/Light Theme**: Toggle between dark and light modes for comfortable viewing
- **Copy-Paste Friendly**: Generated ASCII art is ready to be pasted into your code or documentation
- **Browser-Based**: No installation required - works directly in your web browser
- **Signal Grouping Support**: Handles nested signal groups and hierarchical displays

## Usage

1. Visit [https://wipeseals.github.io/asciidrom/](https://wipeseals.github.io/asciidrom/)
2. Enter your WaveDrom JSON in the input area (a sample is provided by default)
3. Click "Convert" or press `Ctrl+Enter` to generate ASCII art
4. Copy the ASCII output and paste it wherever you need it

### Example

**WaveDrom JSON Input:**
```json
{
  signal: [
    { name: "clk", wave: "p..P..p..P..p" },
    { name: "req", wave: "0.1..0....10." },
    { name: "ack", wave: "0..1..0..1.0." }
  ]
}
```

**ASCII Art Output:**
```
clk | _/¯¯¯¯¯¯¯_/¯¯¯¯¯¯¯_/¯¯¯¯¯¯¯_/¯¯¯¯¯¯¯_/¯
req | _______/¯¯¯¯¯¯¯¯\______________/¯¯\____
ack | __________/¯¯¯¯¯¯¯¯\________/¯¯¯¯¯\____
```

## Installation

No installation required! Asciidrom runs entirely in your web browser. Simply visit the live demo link above.

For local development:

1. Clone this repository:
   ```bash
   git clone https://github.com/wipeseals/asciidrom.git
   ```

2. Open `index.html` in your web browser

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request. For major changes, please open an issue first to discuss what you would like to change.

## Related Projects

- **[WaveDrom](https://wavedrom.com/)**: The original digital timing diagram rendering engine that inspired this project
- **[WaveDrom Editor](https://wavedrom.com/editor.html)**: Official WaveDrom online editor for creating visual timing diagrams

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Acknowledgments

- Thanks to the [WaveDrom](https://wavedrom.com/) project for creating the excellent timing diagram format
- Built with modern web technologies for a seamless user experience