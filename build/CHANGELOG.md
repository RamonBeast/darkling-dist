# Darkling v0.1.0 Release Notes

*January 1, 2026*

## Summary

This release focuses on **multiplay**, **security and convenience**, adding encrypted server connections, automatic update checks, and improved authentication.

---

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

