# Prism Desktop

Prism is packaged as a Windows desktop application using Tauri 2.

## Install from Releases

Open [GitHub Releases](https://github.com/APGSwizzVR/Prism/releases/latest) and download the `*-setup.exe` installer. Run it and follow the installation prompts. The MSI is available for managed installs.

## Build locally

Install Node.js 22+ and Rust from https://rustup.rs/, then:

```powershell
npm install
npm run tauri:build
```

The NSIS installer and MSI are created under `src-tauri/target/release/bundle/`.

## Automated releases

Go to Actions → **Build Prism Windows installer** → Run workflow. Choose a new version tag such as `v0.1.0`. GitHub Actions builds the NSIS `.exe` installer and MSI on a Windows runner and publishes both in Releases.

## Current status

This is an installable desktop preview. Chat interactions are local to the current session. Persistent accounts, synced messages/files, live voice and billing are not connected in this desktop build yet.
