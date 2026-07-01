# Wowwie User Guide

Wowwie helps you organize short audio **samples**, longer **composite samples**, and **beats** into **WOW Crates**, then download a crate to your WOW machine so it plays audio in the order you arranged.

This guide reflects the current app (macOS-v1.1).

---

## What You Need

- **iPhone, iPad, or Mac** running Wowwie
- **MP3 or WAV** audio files on your device or computer
- **WOW machine** (USB storage device) for downloading crates — download is available on **Mac** when the device is connected

On first launch, Wowwie may ask for **microphone access** if you plan to record samples.

---

## Navigating the App

Wowwie has four main sections:

| Section | Purpose |
|--------|---------|
| **WOW Crates** | Create crates, add audio, preview contents, download to the WOW machine |
| **Composite Samples** | Build multi-sample audio files from your sample library |
| **Beats** | Manage beat files for your crates |
| **Samples** | Record or link short audio clips |

**On Mac:** use the sidebar on the left to switch sections.

**On iPhone/iPad:** use the tab bar at the bottom.

---

## Terminology

| Term | Meaning |
|------|---------|
| **Sample** | A short audio clip (typically 1–3 seconds). Used as building blocks and can be added to crates directly. |
| **Composite sample** | A single exported audio file made from one or more samples with **1-second gaps** between them. Maximum length: **30 seconds**. |
| **Beat** | A longer audio file used as backing rhythm. Maximum length: **2.5 minutes**. |
| **WOW Crate** | A named collection of **samples and/or composite samples** plus **beats**, arranged in the order you want them on the WOW machine. |

In crate lists, composite samples are marked with a **waveform icon**; regular samples show a small gray dot.

---

## Samples

The **Samples** page is your library of short audio clips.

### Record a new sample

1. Open **Samples**.
2. Tap or click **Record**.
3. Tap or click **Stop** when finished (recordings are limited to **30 seconds**).
4. The **Save Sample** screen opens with a waveform and trim controls.
5. Adjust the start/end handles to trim the clip, enter a name, then save.

Recording always saves a new sample. Existing samples in the list cannot be re-trimmed from this page.

### Add files from your computer

1. Tap or click **Add Files**.
2. Select one or more **MP3 or WAV** files.

**Rules for added samples:**
- Files must be **30 seconds or shorter**.
- Longer files are rejected with an error and are **not** added.
- Wowwie **links** to files on your computer rather than copying them, so your library stays in sync with the original files.

### Manage samples in the list

Each row shows the name, duration, and controls:

| Control | Action |
|---------|--------|
| **Play / Stop** | Preview the sample |
| **Trash** | Remove from Wowwie (does not delete the original file on your computer) |

**Rename:** swipe right on iPhone/iPad, or use the context menu (long press / right-click).

**Remove:** use the trash button, swipe left, or the context menu. Confirm when prompted.

---

## Composite Samples

The **Composite Samples** page lets you combine samples into one exported WAV file.

### Create a new composite sample

1. Open **Composite Samples**.
2. Click **New Composite Sample**.
3. Drag samples from the **Samples List** onto the timeline, or drag them into the **Drop Sample** area.
4. Watch the duration counter — the total cannot exceed **30 seconds** (including 1-second gaps between clips).
5. Click **Save Composite Sample**, enter a name, and confirm.

### Edit an existing composite sample

1. Select a composite sample from **Composite Samples List**.
2. Click **Edit Composite Sample**.
3. Add, remove, or rearrange samples on the timeline.
4. Click **Save Composite Sample** to re-export the file.

### Preview and delete

- Use **Play / Stop** on any composite sample in the list to preview it.
- **Delete:** trash icon on Mac, swipe or context menu on iPhone/iPad. This removes the exported file and removes it from any crates that used it.

---

## Beats

The **Beats** page works like Samples, but for longer rhythm files.

### Add beats

1. Open **Beats**.
2. Click **Add Files**.
3. Select **MP3 or WAV** files.

**Rules for beats:**
- Files must be **2.5 minutes (150 seconds) or shorter**.
- Files are **linked** from your computer, not copied.

### Manage beats

- **Play / Stop** to preview.
- **Remove** with the trash button, swipe, or context menu. Removing a beat from Wowwie does not delete the original file on your computer.

---

## WOW Crates

Crates are how you package audio for the WOW machine.

### Create a crate

1. Open **WOW Crates**.
2. Click **New Crate**.
3. Enter a name on the **Edit Crate** screen.
4. Add samples and beats (see below).
5. Click **Save**.

### Edit a crate

1. Select a crate in **Crate List**.
2. Click **Edit Crate**.

The edit screen has two areas for **Samples** and **Beats**:

#### In this crate
Shows what is currently in the crate. This list is scrollable and supports:
- **Drag to reorder** — order matters on the WOW machine
- **Minus button** — remove an item from the crate
- **Drop zone** — drag items from the “Available to add” list
- **Play** — preview any item

#### Available to add
Shows samples, composite samples, and beats not yet in this crate:
- Click the **+** button to add an item
- Or drag an item into the “In this crate” area or drop zone

Composite samples and regular samples appear together in the samples section. Use the waveform icon to tell them apart.

Repeat the same workflow for the **Beats** section.

### Preview a crate on the main page

Select a crate in **Crate List** to see its **Samples List** and **Beats List** in the panel below. Use the play buttons to preview without opening the editor.

### Delete a crate

- **Mac:** trash icon next to the crate name
- **iPhone/iPad:** swipe left or use the context menu

Deleting a crate does not delete the underlying audio files from your Samples, Composite Samples, or Beats libraries.

---

## Download to WOW Machine (Mac)

When your WOW machine is plugged in via USB, Wowwie detects it automatically (the device must have `samples` and `beats` folders at its root).

### Download steps

1. Connect the WOW machine to your Mac.
2. Open **WOW Crates**.
3. Select the crate you want to download.
4. Click **Download to WOW** (visible only when the device is connected).
5. Wait for the download to finish.
6. When prompted, **restart the WOW machine** to use the new audio.

### What the download does

- Writes crate **samples and composite samples** to the WOW device’s **`samples`** folder
- Writes crate **beats** to the WOW device’s **`beats`** folder
- **Clears** existing files in those two folders first, so only the selected crate’s audio remains
- Uses file timestamps so the WOW machine plays items in the **same order** as your crate lists
- **Ejects** the device when finished

The app does not modify any other folders on the WOW machine.

### Playing audio on the WOW machine

- Press the **sample** button on the device to step through samples in order.
- Press the **beat** button to step through beats in order.
- Playback cycles back to the first item after the last.

Because order is determined by how files were written to the device, arrange your crate lists carefully before downloading.

---

## Audio Limits (Quick Reference)

| Type | Max duration | Format |
|------|--------------|--------|
| Sample (recorded or added) | 30 seconds | WAV (recorded), MP3/WAV (linked) |
| Composite sample | 30 seconds total (includes 1s gaps) | WAV (exported) |
| Beat | 2.5 minutes | MP3/WAV (linked) |

---

## Tips

- **Build samples first**, then composite samples, then add everything to crates.
- **Name your files clearly** — those names appear on the WOW device after download.
- **Preview often** using the play buttons in any list.
- **Link, don’t duplicate** — adding files from your computer keeps a reference to the original; removing from Wowwie does not delete the source file.
- **Order matters** — reorder items in a crate before downloading to control playback order on the WOW machine.

---

## Troubleshooting

| Problem | What to try |
|---------|-------------|
| **Download to WOW** button missing | Connect the WOW machine to your Mac. The button only appears when the device is detected. |
| Sample file rejected when adding | Check that the file is **30 seconds or shorter** and is MP3 or WAV. |
| Beat file rejected when adding | Check that the file is **2.5 minutes or shorter** and is MP3 or WAV. |
| Cannot add sample to composite timeline | The composite sample would exceed **30 seconds**. Remove or shorten clips first. |
| File already in list | You are trying to link the same file twice. |
| Recording does not work | Allow microphone access in System Settings / iOS Settings. |
| Linked file won’t play | The original file may have been moved or deleted on your computer. Re-add it from its new location. |
| Download failed | Keep the WOW machine connected, ensure it is not open in another app, and try again. You may need to eject it manually if auto-eject fails. |

---

## Typical Workflow

1. **Record or add samples** on the Samples page.
2. **Build composite samples** (optional) on the Composite Samples page.
3. **Add beats** on the Beats page.
4. **Create a WOW Crate** and add the samples, composite samples, and beats you want.
5. **Reorder** items in the crate to match how you want them on the device.
6. **Connect the WOW machine** to your Mac and click **Download to WOW**.
7. **Restart the WOW machine** and play.

---

*For technical integration details about the WOW device, see [wow_integration.md](wow_integration.md).*
