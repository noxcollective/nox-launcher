# Nox Launcher

## Overview

**Nox Launcher** is a decentralized reader for manga, manhwa, manhua, comics, web novels, light novels, and novels, designed to deliver high performance, security, and flexibility. Built with modern technologies like **Rust**, **Tauri**, **Next.js (SSG)**, and **shadcn/ui**, Nox Launcher leverages torrent-based and cached content propagation, providing a fast and seamless experience.

## Key Features

- **Decentralization**: Content propagation via torrents and distributed caches.
- **Customization**: Support for custom repositories and configuration via `.toml` files.
- **Security**: Integration with VPNs and custom proxies.
- **Internationalization**: Supports Brazilian Portuguese and English, with translations managed through `.toml` files.
- **Monetization**: Content creators can benefit from cryptocurrency donations and other monetization methods.
- **Modern Interface**: Built with shadcn/ui and Tailwind CSS.
- **Supported Platforms**: Available for Windows, Linux, macOS, Android, iOS, and Web.

## Technologies Used

- **Rust**: Robust and efficient backend.
- **Tauri**: Lightweight framework for building desktop applications.
- **Next.js (SSG)**: Static site generation for high performance.
- **shadcn/ui**: User interface components powered by Tailwind CSS.
- **Bun**: A modern and fast JavaScript runtime.

## Project Setup

### Required Dependencies

1. **Rust**: Install Rust via [rustup](https://rustup.rs/).
2. **Bun**: Set up the JavaScript runtime with [Bun](https://bun.sh/).
3. **Tauri CLI**: Install using the command:
   ```bash
   cargo install tauri-cli
   ```
4. **Node.js**: Optional, for tools not yet supported by Bun.

### Project Structure

```plaintext
nox-launcher/
├── src/                  # Next.js frontend
│   ├── app/              # App Folder
│   └── components/       # components
│      └── ui/            # shadcn/ui components
├── src-tauri/            # Rust code for Tauri
│   ├── src/              # Rust code
│   ├── tauri.conf.json   # Tauri configuration
│   └── Cargo.toml        # Cargo.toml
├── config/               # Configuration in .toml files
├── public/               # Public files for Next.js
├── assets/               # Static resources
├── .env                  # Environment variables
├── bun.lockb             # Bun lock file
├── package.json          # Frontend dependencies
└── README.md             # Project documentation
```

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/organization/nox-launcher.git
   cd nox-launcher
   ```

2. Install dependencies:
   ```bash
   bun install
   ```

3. Build the binaries:
   ```bash
   cargo build
   ```

4. Start the development environment:
   ```bash
   bun dev
   ```

## Build and Distribution Strategy

1. **Frontend Build**:
   ```bash
   bun build
   ```

2. **Tauri Build**:
   ```bash
   cargo tauri build
   ```

3. **Distribution**:
   Generate cross-platform installers with:
   ```bash
   cargo tauri build --release
   ```

## Contributions

Contributions are welcome! Please follow these steps to contribute:

1. Fork the repository and create a branch for your feature or fix:
   ```bash
   git checkout -b my-feature
   ```
2. Test your changes locally.
3. Submit a pull request with a clear description.

## License

Nox Launcher is licensed under the [MIT License](LICENSE).

