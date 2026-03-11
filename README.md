# Waveform Studio

Offline waveform viewer for Tektronix `WFM#003` and Keysight `H5` files.

## Features

- Import multiple `.wfm` and `.h5` files
- Overlay channels with per-channel color, label, scale, and offset
- Oscilloscope-style navigation, zooming, and panning
- Cursor pairs for `X`, `Y`, `XY`, and follow mode
- Automatic measurements for the active channel
- CSV export for visible range or sampled full-range data
- Single-file HTML app with local sample data

## Run

Open [index.html](./index.html) in a modern browser.

If your browser blocks local file access for some H5 workflows, serve the folder locally:

```powershell
python -m http.server 8000
```

Then visit `http://127.0.0.1:8000/`.

## Repository Layout

- `index.html`: main app
- `data/`: sample waveform files

## License

MIT
