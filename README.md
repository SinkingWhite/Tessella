# Tessella

像素级切图验证工具：切图、拼回验证、接缝检查，一个 HTML 文件就能用。

A single-file web tool for pixel-perfect image slicing and verification.

Import an image, slice it into 2 / 3 / 4 / 6 / 9 / 12 / 16 parts (or a custom grid), and verify that the slices reassemble exactly — pixel for pixel, seam for seam.

## Features

- **Slice** — presets for 2, 3, 4, 6, 9, 12, 16 parts plus a custom columns × rows grid; remainder pixels are distributed to earlier slices so integer pixels always sum exactly
- **Verify** — three automatic checks with numbers: coverage integrity, pixel-level reassembly comparison (RGBA diff count, max channel diff, mean error, diff image, flicker compare), and seam fit measurement (coordinate gap, on-screen gap, 10× magnified seam view)
- **Export** — PNG (lossless), JPEG (quality slider, auto white background), or WebP, with a live estimate of total export size vs. the original
- **Trilingual UI** — 简体中文 / 繁體中文 / English, switchable in one click
- **No build, no backend** — a single HTML file; open it in a browser and it works

## Usage

Open `index.html` in any modern browser. Drag & drop an image (or paste with Ctrl+V), pick a slice mode, and the verification runs automatically.

## License

MIT
