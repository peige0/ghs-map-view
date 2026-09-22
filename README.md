# GHS Map Viewer

A lightweight, browser-based analyzer for Green Hills linker `.map` and linker-script `.ld` files, focused on embedded firmware memory visualization.

## Features

- Parse Green Hills linker map files locally in the browser
- Parse linker-script MEMORY regions and section-to-region mappings
- Visualize Flash/RAM usage by memory region
- Address layout view with free holes
- Explorer for Region / Section / Module / Symbol navigation
- Treemap views for symbols, modules, and sections
- Sort by address, size, free space, usage, largest hole, or name
- Search sections, modules, and symbols
- Optional memory-header parsing for linker macros
- Manual region override when origin/length expressions cannot be resolved
- Export memory-region statistics to CSV
- No upload: analyzed files remain in the browser

## Usage

1. Open `index.html` in a modern browser.
2. Load or drag in a Green Hills `.map` file and the corresponding linker `.ld` file.
3. Optionally add a memory definition `.h` or `.txt` file.
4. Use the tabs to inspect regions, address layout, symbols, modules, and treemaps.

## Project status

This is an early open-source release extracted from a practical embedded-development workflow. The current parser targets Green Hills map/linker output and will be expanded for more toolchains and file variants.

## Roadmap

- Package as a VS Code extension
- Add anonymized sample files and regression tests
- Improve parser tolerance across Green Hills versions
- Add GCC / IAR linker-map support
- Add richer bank/block visualization
- Add import/export of analysis sessions

## Privacy

All parsing is performed locally in your browser. Input files are not uploaded by this tool.

## License

MIT
