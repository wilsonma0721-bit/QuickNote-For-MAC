# QuickNote
中文🇨🇳Version

轻量级 macOS 原生悬浮便签与临时文件暂存工具。

常驻屏幕顶层的半透明毛玻璃面板，上半部分为纯文本实时笔记编辑器，下半部分为临时文件暂存区（Shelf），支持全域快捷键秒开秒关。

## 核心特性

* **轻量原生**：纯 AppKit 构建，无第三方依赖；常驻菜单栏（Menu Bar），不占 Dock 空间。
* **即时纯文本笔记**：打开即聚焦输入框，输入自动原子落盘（`~/Library/Application Support/QuickNote/note.md`），支持完整的撤销/重做与一键复制。
* **临时文件暂存区（Shelf）**：
  * 支持将文件、图片、PDF 拖入面板或直接 `Cmd + V` 粘贴收纳。
  * 收纳采用复制机制，原文件不受影响；拖出到其他应用同样为复制。
  * 支持空格键 Quick Look 快速预览、右键在 Finder 中显示，删除统一移入废纸篓可随时救回。
* **自由窗口交互**：
  * 顶部标题栏自由拖拽（支持跨多显示器），八方向边缘与角落自由缩放。
  * 可拖动分隔线自由调整笔记区与暂存区的上下比例。
  * 独立调节毛玻璃背景透明度（20%–100%，双击恢复默认），文字与内容始终清晰。
* **全域快捷键**：默认 `⌘N` 唤醒/隐藏面板，支持自定义组合键与冲突自动回退提示。

## 常用快捷键

| 快捷键 | 作用域 | 功能 |
| :--- | :--- | :--- |
| `⌘ + N` | 全局 | 显示 / 隐藏悬浮面板（可在设置中修改） |
| `⌘ + +` / `⌘ + -` | 面板内 | 等比例放大 / 缩小窗口 |
| `⌘ + 0` | 面板内 | 重置窗口至默认尺寸（360×480） |
| `⌘ + V` | 面板内 | 剪贴板为文件/图片时自动收入暂存区，纯文本则正常粘贴 |
| `Space` | 暂存区 | 打开 / 关闭 Quick Look 预览 |
| `Delete` | 暂存区 | 将选中暂存文件移入废纸篓 |
| `Return` | 暂存区 | 使用系统默认应用打开选中文件 |

## 环境要求与构建

* **系统要求**：macOS 13.0 及以上
* **构建方式**：使用 Xcode 打开项目或通过 Swift / `xcodebuild` 直接编译运行（无需额外包管理工具）。

## 数据存储位置

* **笔记内容**：`~/Library/Application Support/QuickNote/note.md`
* **暂存文件**：`~/Library/Application Support/QuickNote/Shelf/`
* # QuickNote
ENGLISH🇬🇧 Version
A lightweight, native macOS floating scratchpad and temporary file shelf.

Always-on-top translucent frosted-glass panel featuring a real-time plain-text note editor on top and a temporary file staging area (Shelf) on the bottom, toggled instantly via a global hotkey.

## Key Features

* **Lightweight & Native**: Built purely with AppKit with zero third-party dependencies. Lives quietly in the Menu Bar without cluttering your Dock.
* **Instant Plain-Text Notes**: Automatically focuses the editor on launch, saves atomically in real time (`~/Library/Application Support/QuickNote/note.md`), and supports full Undo/Redo and one-click copy.
* **Temporary File Shelf**:
  * Drag and drop files, images, or PDFs anywhere onto the panel, or simply paste with `Cmd + V`.
  * Non-destructive copy-in/copy-out workflow—original files remain untouched, and deleted items are safely moved to the Trash.
  * Press `Space` for Quick Look preview, or right-click to reveal items in Finder.
* **Flexible Window Controls**:
  * Drag the top title bar across multiple displays and resize freely from all 8 edges and corners.
  * Adjust the split ratio between the note editor and file shelf via a draggable divider.
  * Customize frosted-glass background opacity (20%–100%, double-click slider to reset) while keeping text and icons crisp.
* **Global Hotkey**: Toggle visibility anywhere with `⌘N` (customizable with automatic conflict detection and fallback).

## Shortcuts

| Shortcut | Scope | Action |
| :--- | :--- | :--- |
| `⌘ + N` | Global | Show / Hide floating panel (customizable in settings) |
| `⌘ + +` / `⌘ + -` | In-Panel | Scale window size proportionally |
| `⌘ + 0` | In-Panel | Reset window to default size (360×480) |
| `⌘ + V` | In-Panel | Add files/images from clipboard to Shelf, or paste plain text into editor |
| `Space` | File Shelf | Toggle Quick Look preview |
| `Delete` | File Shelf | Move selected item(s) to Trash |
| `Return` | File Shelf | Open selected item(s) with default app |

## Requirements & Build

* **Requirements**: macOS 13.0 or later
* **Build**: Open the project in Xcode or compile directly using Swift / `xcodebuild` (no package manager required).

## Data Storage

* **Notes**: `~/Library/Application Support/QuickNote/note.md`
* **Staged Files**: `~/Library/Application Support/QuickNote/Shelf/`
