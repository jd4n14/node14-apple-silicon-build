# Node.js 14 Apple Silicon (arm64) Unofficial Build

This project provides **unofficial prebuilt binaries of Node.js 14** for **macOS on Apple Silicon (arm64)**.

The binaries are built to fill the gap left by the official Node.js distribution, which does not provide native support for arm64 for some versions of Node.js 14.

## 🔧 Installation with `fnm`

You can install and use these builds with [`fnm`](https://github.com/Schniz/fnm), the fast Node.js version manager.

### ✅ Step-by-step instructions

1. **Clone this repository locally**:

   ```bash
   git clone git@github.com:jd4n14/node14-apple-silicon-build.git
   cd node14-apple-silicon-build
   ```

2. **Start a local HTTP server** from the project directory:

   ```bash
   python3 -m http.server
   ```

3. **Install Node.js 14 (arm64) using `fnm`**, pointing it to the local server:

   ```bash
   fnm install 14 --arch arm64 --node-dist-mirror http://localhost:8000/release
   fnm use 14
   ```

4. **Verify that you're using the correct architecture**:

   ```bash
   node -p "process.arch"
   # 'arm64'
   ```

This will install the native ARM64 build of Node.js 14.21.3 provided in this repo.

---

## 🌐 Other useful sources

- [Official Node.js Releases](https://nodejs.org/dist/)
- [Official Nightly Builds](https://nodejs.org/download/nightly/)
- [Unofficial Linux builds for special architectures](https://unofficial-builds.nodejs.org/download/release)

---
> ⚠️ Disclaimer: These builds are unofficial and not supported by the Node.js core team. Use them at your own discretion.
