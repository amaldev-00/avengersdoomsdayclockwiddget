# Doomsday Countdown (Android)

A small native Android Studio project for a dark, rounded neon-green countdown to **Avengers: Doomsday**.

## Features
- Full-screen countdown that updates every second while the app is open.
- Home-screen widget with the same rounded green panel and `UNTIL AVENGERS: DOOMSDAY` caption.
- Editable target date and time from inside the app.
- Default target: **18 December 2026 at 12:00 AM**, using the phone's local timezone. Change it in-app if the official release time/date changes or you prefer another target.
- No network access, account, analytics, or special permissions.

## Build and install
1. Install **Android Studio** on a computer.
2. Extract this ZIP and open the `DoomsdayCountdown` folder in Android Studio.
3. Allow Gradle sync to finish (Android Studio will download the Android Gradle Plugin and SDK components if needed).
4. Connect your Android phone with USB debugging enabled, or choose **Build → Build Bundle(s) / APK(s) → Build APK(s)**.
5. Install the generated debug APK on your phone.
6. To add the widget, long-press an empty area of the home screen → **Widgets** → **Doomsday Countdown**.

## Widget refresh note
The app screen updates once per second. Android home-screen widgets are not designed for guaranteed per-second updates. This widget requests an inexact refresh about once per minute; Android/Realme battery management may delay it. The countdown remains accurate whenever it refreshes and immediately when you open the app.

## Lock screen note
This project registers a standard Android home-screen widget. Third-party lock-screen widget support is device/firmware-specific; Realme UI 7 may not expose ordinary app widgets in its lock-screen widget picker. The app cannot force a widget onto the lock screen. Check Settings → Home screen, Lock screen & style → Lock screen customization/widgets (wording may vary).

## Design
The interface uses a pure-black canvas, dark panel, rounded fluorescent-green outline, monospaced digits, thin divider, and the requested caption inside the same panel. It is an original fan-made countdown utility and is not affiliated with Marvel.

## Get the APK without Android Studio
1. Create a free GitHub account and a new repository, then upload this whole folder (including the hidden `.github` folder).
2. Open the repo's **Actions** tab → **Build APK** → wait about 3–5 minutes for the green tick.
3. Open the finished run → **Artifacts** → download **DoomsdayCountdown-APK**, unzip it, and install `app-debug.apk` on your phone (allow "Install unknown apps" when asked).
