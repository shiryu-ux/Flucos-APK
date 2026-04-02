# Flucos — Your Focus, Your Flow

Flucos is an Android focus app designed to help users minimize phone distractions during study or work sessions. It features two distinct modes tailored for different needs — **Control** for parental oversight and **Mastery** for self-disciplined focus.

---

## Features

###  Focus Lock
- Custom countdown timer with hours and minutes picker
- Screen pinning during focus sessions to prevent distractions
- Back button blocked during active sessions
- Emergency Escape with **2 attempts per week**

###  Allowed Apps
- Select up to **5 apps** that can be used during focus sessions (e.g. GCash, Messenger, Gmail)
- App icons displayed on the Lock screen for quick access
- Strict Mode toggle — disables all allowed apps for full focus

###  Alarm
- Set alarms with custom start time, duration, and label
- Repeat days selection (S M T W T F S)
- Two alarm modes: **Notify Only** and **Auto Lock**
- Vibration when alarm rings

###  Analytics
- Monthly calendar view with session tracking
- Orange highlight on days with completed focus sessions
- Streak counter with 🔥 emoji
- Today / Month / Total session stats in minutes

###  Settings
- **Allowed Apps Permission** — toggle strict focus mode
- **Vibrate When Complete** — vibrate when timer finishes
- **Do Not Disturb** — silence notifications during focus
- **Stable Lock Mode** — keep screen on during focus
- **Anti-Delete Protection** — prevent app uninstall (Control mode only)
- **Emergency Escape** — toggle with weekly attempt counter
- **Switch Mode** — switch between Control and Mastery
- **Change Password** — update Control mode password (Control mode only)

###  Two Modes

#### Control Mode
Designed for parents who want to manage their child's digital behavior.
- Requires a **6-digit PIN** to complete focus sessions
- Anti-Delete Protection available
- Change Password option in Settings

#### Mastery Mode
Built for students and professionals who want to minimize phone usage.
- No password required
- Pure self-discipline focus timer

---

## Onboarding Flow
1. Splash screen
2. Grant **Accessibility Service** permission (required for app blocking)
3. Grant **Display Over Other Apps** permission (required for overlay)
4. Select allowed apps (up to 5)
5. Choose **Control** or **Mastery** mode
6. Start focusing!

---

## Tech Stack
- **Language:** Java
- **Min SDK:** Android 8.0 (API 26)
- **Target SDK:** Android 14 (API 34)
- **Architecture:** Single Activity + Multiple Activities
- **Storage:** SharedPreferences
- **UI:** Material Design 3

---

## Permissions Required
| Permission | Purpose |
|---|---|
| `VIBRATE` | Vibration on session complete and alarm |
| `SCHEDULE_EXACT_ALARM` | Scheduling alarms |
| `USE_EXACT_ALARM` | Exact alarm timing |
| `ACCESS_NOTIFICATION_POLICY` | Do Not Disturb control |
| `SYSTEM_ALERT_WINDOW` | Display over other apps |
| `RECEIVE_BOOT_COMPLETED` | Reschedule alarms after reboot |
| `QUERY_ALL_PACKAGES` | Show installed apps list |
| `BIND_ACCESSIBILITY_SERVICE` | Block non-allowed apps during focus |
| `BIND_DEVICE_ADMIN` | Anti-Delete Protection |

---

## Installation
1. Clone the repository
```bash
git clone https://github.com/yourusername/flucos.git
```
2. Open in **Android Studio**
3. Build and run on a physical device (emulator not recommended for accessibility features)

---

## Screenshots
> Add your screenshots here

---

## Known Limitations
- App blocking via Accessibility Service requires the user to manually enable it once in Android Settings
- Alarm scheduling may vary across Android manufacturers (Xiaomi, Samsung, Oppo, etc.)
- Display Over Other Apps permission must be granted manually on Android 10+

---

## License
This project is for educational and personal use only.

---

## Developer
Built with ❤️ by [Hive]
