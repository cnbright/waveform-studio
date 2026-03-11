# Waveform Studio

中文为主，English follows below.

## 中文说明

Waveform Studio 是一个单文件离线示波器波形工作台，用于查看和测量 Tektronix `WFM#003` 与 Keysight `H5` 存储波形文件。

### 功能特性

- 支持同时导入多个 `.wfm` 与 `.h5` 文件
- 支持多通道叠加显示，并可分别设置颜色、左侧标签、`Y Scale`、`Y Offset`
- 支持示波器常见交互：滚轮缩放、拖拽平移、框选放大、双击全局自适应
- 支持 `X`、`Y`、`XY`、跟随四类游标
- 支持主测量通道自动测量
- 支持导出当前视图 CSV 和全量抽点 CSV
- 单文件 HTML 交付，可离线使用

### 测量说明

- 自动测量基于当前主测量通道
- 可切换“当前视图测量”与“全波形测量”
- 上下调整波形 `Y Offset` 仅影响显示位置，不影响自动测量和游标测量结果

### 运行方式

直接用现代浏览器打开 [index.html](./index.html) 即可。

如果浏览器对本地文件访问有限制，建议在仓库目录启动本地静态服务：

```powershell
python -m http.server 8000
```

然后访问 `http://127.0.0.1:8000/`。

### 仓库结构

- `index.html`：主应用入口
- `data/`：示例波形文件

### 开源协议

MIT

---

## English

Waveform Studio is a single-file offline oscilloscope waveform workbench for viewing and measuring Tektronix `WFM#003` and Keysight `H5` waveform files.

### Features

- Import multiple `.wfm` and `.h5` files
- Overlay channels with per-channel color, left-side label, `Y Scale`, and `Y Offset`
- Oscilloscope-style navigation with wheel zoom, drag pan, box zoom, and double-click autoscale
- Cursor tools for `X`, `Y`, `XY`, and follow mode
- Automatic measurements for the active measurement channel
- CSV export for the visible range or sampled full-range data
- Single-file HTML app for offline use

### Measurement Notes

- Automatic measurements are based on the active measurement channel
- Switch between measurement on the current view and the full waveform
- Moving `Y Offset` changes display position only and does not change measurement results

### Run

Open [index.html](./index.html) in a modern browser.

If your browser restricts local file access, serve the folder locally:

```powershell
python -m http.server 8000
```

Then open `http://127.0.0.1:8000/`.

### Repository Layout

- `index.html`: main app entry
- `data/`: sample waveform files

### License

MIT
