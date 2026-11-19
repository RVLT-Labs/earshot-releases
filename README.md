<div align="center">
  <img src="assets/earshot.png" alt="Earshot" width="96" height="96">

  <h1>Earshot</h1>
  <p><strong>Live transcription for the crew behind the show.</strong></p>
  <p>Follow your comms channels on a desktop, phone or tablet.<br>Speech recognition runs on your host computer.</p>

  <p>
    <a href="https://github.com/RVLT-Labs/earshot-releases/releases/latest"><strong>Download Earshot</strong></a>
    &nbsp;·&nbsp;
    <a href="https://rvlt-labs.github.io/earshot-manual/">Read the manual</a>
    &nbsp;·&nbsp;
    <a href="https://github.com/RVLT-Labs/earshot-releases/releases">Release notes</a>
    &nbsp;·&nbsp;
    <a href="https://rvlt-labs.github.io/earshot-manual/changelog">Changelog</a>
  </p>
  <p>Built by <strong>RVLT</strong> for live-production crews.</p>
</div>

---

![Earshot's live transcript feed, with colour-coded channels, speaker names and audio levels](assets/earshot-feed.png)

*Demo show with sample transcript content.*

## Keep up with the conversation

Earshot turns speech from multiple audio channels into a live, readable transcript. Run it on the computer connected to your audio inputs, then let the crew follow along in a browser on the show network.

- **Read across channels.** Follow a combined Feed, arrange channels in Lanes, or use Focus for a larger view.
- **Catch your name.** Enter your name or keywords under **Display → Personal keyword alerts** to flash only your device and show the matching line. No automation or Armed mode is needed.
- **Bring the crew in.** Phones, tablets and laptops connect through a browser. Only the host needs the desktop app.
- **Recognise speech locally.** Download the speech models during setup, then run them on your host. Cloud speech and translation are optional and require you to enable them.
- **Correct what you read.** Select words or use the pencil to edit a finished line; admins can remember recurring mishearings. Production cue abbreviations such as “LXQ 912” are expanded for display without changing cue numbers or automation input.
- **Get earlier drafts.** Optionally use Moonshine tiny for English drafts while keeping the main model for finished text. Setup includes transcription timing and guided voice enrollment.
- **Recognise individual voices.** Shared channels can discover voices automatically, split consecutive speakers into separate lines and let you name them later. Optional two-voice overlap separation is experimental and slower than real time.
- **Run on Apple Silicon.** The Mac speech runtime uses cached processing, tuned model threads and scheduling priorities for live transcription.
- **Find a line again.** Search the transcript archive, add markers and export transcripts.
- **Make it fit your show.** Organise channels into groups and add names and production terms to the glossary.
- **Connect show control.** Build phrase-triggered OSC, MIDI and HTTP actions, with Armed/Safe controls, a test bench and an activity log.

## Download

**[Get the latest release →](https://github.com/RVLT-Labs/earshot-releases/releases/latest)**

**macOS Apple Silicon: v0.5.0. Windows and Linux updates are on hold at v0.4.0.** Check the release notes before installing or updating.

| Your computer | Download |
|---|---|
| **macOS · Apple Silicon** | [DMG installer](https://github.com/RVLT-Labs/earshot-releases/releases/download/v0.5.0/Earshot_0.5.0_aarch64.dmg) |
| **Windows · 64-bit · v0.4.0** | [EXE installer](https://github.com/RVLT-Labs/earshot-releases/releases/download/v0.4.0/Earshot_0.4.0_x64-setup.exe) · [MSI installer](https://github.com/RVLT-Labs/earshot-releases/releases/download/v0.4.0/Earshot_0.4.0_x64_en-US.msi) |
| **Linux · x86_64 · v0.4.0** | [AppImage](https://github.com/RVLT-Labs/earshot-releases/releases/download/v0.4.0/Earshot_0.4.0_amd64.AppImage) · [DEB](https://github.com/RVLT-Labs/earshot-releases/releases/download/v0.4.0/Earshot_0.4.0_amd64.deb) · [RPM](https://github.com/RVLT-Labs/earshot-releases/releases/download/v0.4.0/Earshot-0.4.0-1.x86_64.rpm) |

There is no Intel Mac build. Linux packages are built on Ubuntu 22.04. GitHub's **Source code** archives contain this downloads page and its images; install one of the packages above.

### Updates

Earshot v0.3.0 adds **Check for Updates…** to the tray icon's context menu and the macOS Earshot menu. It checks GitHub Releases after startup and every six hours, with **Update now**, **Not now**, and **Don't remind me for this update** choices. Update downloads are checked against an updater signature before installation.

**Upgrading from v0.2.0 or earlier?** Install the appropriate package above manually once. Future versions can update in-app on macOS, Windows and Linux AppImage installations. Linux DEB/RPM installations use the package manager.

### Before you install

The macOS app is ad-hoc signed but not notarised; Windows installers are not Authenticode-signed. Updater artifacts have separate verified signatures. macOS may require approval in **System Settings → Privacy & Security**. Windows may show a SmartScreen warning. Read the release notes for instructions.

The v0.5.0 Mac build passed its headless startup check and packaged-app checks on Apple Silicon. The older v0.4.0 Windows and Linux packages passed headless startup checks; their installer interfaces and desktop windows have not yet been tested. Noisy comms, overlapping voices and isolated commands can still produce missed or incorrect words. Test your actual audio feed and show setup before relying on it in production.

Verify your download against the checksums for its version: [macOS v0.5.0](https://github.com/RVLT-Labs/earshot-releases/releases/download/v0.5.0/SHA256SUMS.txt) or [Windows/Linux v0.4.0](https://github.com/RVLT-Labs/earshot-releases/releases/download/v0.4.0/SHA256SUMS.txt).

## Your first session

1. **Install and open Earshot** on the computer connected to your audio inputs.
2. **Install the recommended speech models** in **Setup → Models** while you have internet access.
3. **Choose your inputs** in **Setup → Patch**, then check that speech appears in the Feed.
4. **Set access for your crew** in **Setup → Access** and share **Address for the crew**. They open it in a browser on the same network.

Keep the show **Safe** while setting up and testing automations. The manual covers access controls, model downloads, show control and the current limits.

**[Open the user manual →](https://rvlt-labs.github.io/earshot-manual/)**

---

This repository is the public home for Earshot installers, release notes and download information. The application source is maintained in a separate private repository.
