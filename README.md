 <div align="center">

# 🐍 0xM4mba — Fastfetch Configuration

**A custom Linux terminal setup with a MAMBA-inspired aesthetic.**

`Fastfetch` · `Linux` · `JSONC` · `Terminal Customization`

</div>

---

## 🐍 About

Welcome to my Fastfetch configuration repository!

This repository contains my personal Fastfetch setup, customized with a **MAMBA-inspired hacker aesthetic**. It features a custom logo, organized system information, red accents, and a clean terminal layout.

The goal is to make the terminal look unique while keeping system information simple, readable, and useful.

## ⚡ Features

- 🐍 **Custom branding** — MAMBA-inspired terminal identity.
- 🎨 **Custom color scheme** — vermilion red, warm white, and muted tones.
- 🖼️ **Custom logo** — image-based logo using the Kitty graphics protocol.
- 💻 **System information** — OS, kernel, shell, and package count.
- ⚙️ **Hardware information** — CPU, GPU, memory, and disk usage.
- 📊 **Resource indicators** — colored indicators for different usage levels.
- 🧩 **Custom modules** — organized `VITALS` and `SYSTEM` sections.
- 🛠️ **JSONC configuration** — easy to customize and maintain.

## 🖥️ Preview

<!-- Add your Fastfetch screenshot here -->

![Fastfetch Preview](assets/fastfetch-preview.png)

> Replace the image path above with the actual location of your screenshot.

## 📂 Repository Structure

```text
.
├── config.jsonc
├── kataa.png
└── README.md
```

## 🧰 Requirements

- [Fastfetch](https://github.com/fastfetch-cli/fastfetch)
- A terminal that supports truecolor output
- A compatible terminal supporting the Kitty graphics protocol for the image logo
- The `ryoku` command for the custom OS version display

## 🚀 Installation

**1. Install Fastfetch**

Install Fastfetch using your Linux distribution's package manager or follow the [official installation guide](https://github.com/fastfetch-cli/fastfetch).

**2. Create the configuration directory**

```bash
mkdir -p ~/.config/fastfetch
```

**3. Copy the configuration and logo**

Run these commands from the repository directory:

```bash
cp config.jsonc ~/.config/fastfetch/config.jsonc
cp kataa.png ~/.config/fastfetch/kataa.png
```

**4. Launch Fastfetch**

```bash
fastfetch --config ~/.config/fastfetch/config.jsonc
```

## 🎨 Customization

Edit `config.jsonc` to personalize your setup.

| Setting | Description |
|---|---|
| `logo.source` | Custom logo image path |
| `logo.width` / `logo.height` | Logo dimensions |
| `display.color.keys` | Accent color for system information |
| `display.key.width` | Width allocated to module labels |
| `modules` | Order and content of displayed information |
| `VITALS` | Hardware and resource information |
| `SYSTEM` | OS, kernel, shell, and package information |

The configuration uses a vermilion-red accent (`RGB 226, 52, 42`) with warm off-white text and muted separators.

## 📝 Notes

- The logo path is set to `~/.config/fastfetch/kataa.png`.
- The image display uses the `kitty-direct` protocol, which is not supported by every terminal.
- The OS module displays `DEBAIN` and attempts to retrieve a version using `ryoku version`, falling back to `dev`.
- System information depends on the hardware and software environment where Fastfetch runs.

## 🔗 Credits

- [Fastfetch](https://github.com/fastfetch-cli/fastfetch) — system information tool.
- Configuration and styling by [@0xM4mba](https://github.com/0xM4mba).

---

<div align="center">

**Built for the terminal. Styled by MAMBA.** 🐍

</div>
