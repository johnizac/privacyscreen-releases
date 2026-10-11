# PrivacyScreen

An Android app that dims or patterns your screen so people next to you can't easily read it. It is a software take on Samsung's Privacy Display, for phones that don't have one. Taps, scrolling and typing keep working in the app underneath.

This repository only hosts the downloads. Android 8.0 or later.

## Install

1. On your phone, open the [latest release](https://github.com/johnizac/privacyscreen-releases/releases/latest) and tap the `.apk` file to download it.
2. Open the download. Android asks you to allow installs from your browser; turn that on.
3. Tap **Install**. If Play Protect warns that the app is unknown (it isn't from the Play Store), choose **Install anyway**.
4. Open PrivacyScreen and follow **Finish setup**.

To update, install the newer APK over the old one. Your settings are kept.

## What it does

- **Five looks:** Dim, Lines, Grid, Dots, and Read (everything dimmed except a band you drag up and down).
- **Strength and pattern size sliders**, with a live preview.
- **Turn it on or off from anywhere:** Quick Settings tile, the notification, or the app.
- **Automatic:** turns on when you open apps you choose and off when you leave them.
- **Start after restart:** brings back the last state after the phone reboots.

## Permissions, and why

| Permission | Why |
| --- | --- |
| Display over other apps | Draws the dim layer over other apps. Required. |
| Notifications | Shows the ongoing notification with the Turn off and Change mode buttons. |
| Usage access | Only for automatic mode: tells the app which app is in front. No Accessibility service is used. |
| Run at startup | Only for "Turn back on after the phone restarts". |

On Samsung phones, also set **Settings > Apps > PrivacyScreen > Battery > Unrestricted**, or Samsung may stop the app in the background.

The app has no internet permission: nothing leaves your phone.

## Known limits

- The status bar and navigation bar icons stay bright. Android draws them above every app.
- The overlay doesn't show on the lock screen, on permission dialogs or on some system screens.
- Screenshots and screen recordings include the overlay.
- It can't copy Samsung's hardware, which blocks light by viewing angle. Lines, Grid and Dots get in the way most up close; from a few metres away they blur into a plain dim layer. For onlookers further away, use Read mode, or Dim at high strength with low screen brightness.
- Strength stops at 80%: above that, Android 12+ blocks taps from reaching the app underneath.
