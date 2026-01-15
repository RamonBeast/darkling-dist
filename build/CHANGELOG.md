# Darkling v0.3.0 Release Notes

  *January 15, 2026*

  ## Summary

  This release introduces the migration system, letting you travel to new star systems. It also adds broadcasts, deep space telemetry, LED notifications, power saving mode, and numerous quality-of-life improvements.

  ### Migration System

  - **Travel to new stars**: Migrate your civilization to any neighboring star visible in Astronomy view
  - **Migration costs**: Requires resources to initiate (cost varies by distance and number of Colonies)
  - **Bounce mechanics**: If your destination is occupied when you arrive, you may bounce to a nearby system after a battle on arrival

  ### Broadcast System

  - **Share star coordinates**: Send the location of any star you've discovered to other players
  - **Two broadcast targets**:
    - *To Galaxy*: Broadcast to all players in the universe
    - *To Contact*: Send privately to a specific player from your contacts list
  - **Galaxy broadcast modes**:
    - *Public*: Your identity **is revealed** to all recipients
    - *Anonymous*: Recipients see the coordinates but **not who sent them**
  - **Contact broadcast**: Send coordinates directly to one player
  - **Strategic uses**:
    - Reveal your own star to invite contact (public broadcast of your location)
    - Share intel about other players' positions
    - Send *anonymous* tips without exposing yourself
  - **Creates contacts**: When you receive a broadcast, the star is added to your contacts for easy reference

  ### LED Notifications

  - **Event-based LED alerts**: LED blinks to notify you of important events
    - Probe results and detections
    - Research completions
    - Migration arrivals
    - Incoming broadcasts

  ### Power Save Mode

  - **Auto screen-off**: Display turns off after a period of inactivity
  - **Touch to wake**: Tap the screen to resume

  ### WiFi Improvements

  - **Network scanning**: See available WiFi networks when connecting
  - **Automatic timezone**: Device detects your timezone automatically via WiFi
  - **Better reconnection**: Fixed exponential backoff for more reliable server reconnection

  ### Contacts

  - **Contacts panel**: Added new *Contacts* panel
    - Broadcast targets appear as contacts
    - Player-to-Player broadcast appear as contacts
    - Confirmed Probe discoveries are automatically add to *Contacts*
  - **Relationship-aware labels**: Contact sources now show meaningful context:
    - "Revealed their coordinates" - player introduced themselves
    - "Via [name]" - coordinates forwarded by another player
    - "Anonymous signal" - anonymous broadcast
    - "Detected by probe" - confirmed by your probe

  ### Bug Fixes

  - Fixed astronomy pagination getting out of sync when rapidly navigating
  - Fixed MQTT reconnection causing stack overflow under poor network conditions
  - Fixed WiFi icon changing during network scans while already connected
  - Fixed journal entry text getting clipped
  - Fixed research feedback not displaying correctly
  - Improved toast notification delivery when UI is busy
  - Added support for additional hardware variants (Boya flash chips, inverted touch panels)

  ---

# Darkling v0.2.0 Release Notes

*January 6, 2026*

## Summary
This release focuses on exploration and progression, adding the research system, probe-based intelligence gathering, astronomy mapping, and counter-espionage.

### Journal System
- **Complete event journal implementation** 
  - Track all major game events in a persistent log
  - View probe launches, arrivals, and discoveries
  - Track research completions and milestones

### Research System
- **Technology Tree**: Unlock new capabilities through research
  - **Dark Veil** (I, II, III): Enable and enhance veil protection
  - **Astronomy** (I, II, III): View stars up to 1, 2, or 3 hops away
  - **Espionage** (I, II, III): Improved probe detection accuracy
  - **Counter Espionage** (I, II, III): Detection incoming probes and alter their intelligence
- Research costs resources and takes real-time to complete (only progresses while online)

### Probe & Astronomy System
- **Send Probes**: Launch probes to distant stars to detect enemy civilizations
- **Detection Results**: 
  - Confirmed detection
  - Suspected presence (weak, moderate, or strong signals)
  - Nothing detected
- **Probe Speed**: Probes travel at 6x the speed of normal space travel
- **Astronomy View**: See neighboring stars based on your ASTRONOMY research level

### UI/UX Enhancements
- **Better time formatting** - Human-readable timestamps ("5 min ago", "2 hours ago")
- **Improved descriptions** - Clearer text throughout the interface
- **Signal strength progress bar** - Visual feedback about your Civilization's signal level
- **Lore & Guide** - Added a section with some lore and a mini-guide

### Bug Fixes
- Fixed journal event timestamp parsing for accurate time display
- Fixed probe result handling and notification
- Fixed astronomy cache invalidation when launching probes
- Fixed LOG badge positioning to be visible
- Fixed various MQTT message handling edge cases
- Fixed signal strength progress bar display
- Improved stability and error handling throughout

---

# Darkling v0.1.0 Release Notes

*January 1, 2026*

## Summary

This release focuses on **multiplay**, **security and convenience**, adding encrypted server connections, automatic update checks, and improved authentication.

## New Features

### Multiplayer Universe
- **Multiplayer Universe** - Now active, you can finally play on the same universe all the other players

### Automatic Update Checks
- **Boot-time update detection** - Your device now checks for firmware updates automatically when it starts up
- **Faster update deployment** - No need to wait 30 minutes for periodic checks
- **Smart WiFi triggering** - Update check happens once WiFi connection is established

### Enhanced Security
- **Encrypted MQTT connections (TLS)** - All game server communication is now encrypted for privacy and security
- **Dynamic Security authentication** - Improved authentication system for better account protection
- **Hashed player IDs** - Player identifiers are now cryptographic hashes instead of raw device IDs

## Improvements
- **Better star rendering** - Fixed visual glitches with the central star display
- **More reliable server connection** - Improved MQTT message handling during player registration
- **Cleaner interface** - Reduced unnecessary debug messages for a smoother experience
- **Factory reset** - Hold "boot" button down for 3 seconds to restore to factory settings (wifi data is erased, calibration data is erased, player data *is retained*)

---

# Darkling v0.0.9 Release Notes

*December 29, 2025*

## 🎮 New Features

### ✨ __Realistic Star Colors & Visual Effects__

- __Dynamic Star Appearance__: Stars now display authentic colors based on their stellar classification

  - 🔵 Hot blue-white stars (O/B class) - the most massive and energetic
  - ⚪ Bright white stars (A class) - hot and luminous
  - 🟡 Yellow-white stars (F class) - slightly hotter than our Sun
  - 🟨 Yellow stars (G class) - like our own Sun
  - 🟠 Orange stars (K class) - cooler, long-lived stars
  - 🔴 Red stars (M class) - the coolest, most common stars

- __Star Glow Effects__: Each star class now has appropriate glow and atmospheric effects

- __Real-time Updates__: Star colors change dynamically as you migrate between different star systems

### 🏛️ __Colony-Focused Gameplay__

- __Streamlined Interface__: Cleaner UI shows your colony count and progress

### 🔄 __Improved Game Experience__

- __Better Performance__: Optimized rendering and smoother gameplay
- __Enhanced Connectivity__: More reliable connection to game servers
- __Cleaner UI__: Removed unnecessary information display for better focus on gameplay

## 🛠️ __Quality of Life Improvements__

### 📱 __Device Management__

- __Factory Reset__: Hold the boot button for 3 seconds to reset your device settings while preserving your game progress
- __Auto-Update__: System now checks for updates once every 30 minutes instead of constantly
- __Better Authentication__: More reliable connection to game servers

### 🎨 __Visual Enhancements__

- __Improved Display__: Better color representation and visual effects
- __Optimized UI__: Cleaner interface with focus on important game information

## 🔧 __Under the Hood__

- Improved memory usage and system stability
- Enhanced error handling and recovery
- Better game state synchronization
- Optimized network communication