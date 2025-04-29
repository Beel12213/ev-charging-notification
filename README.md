# EV Charging Notification Blueprint for Home Assistant 🚗⚡

Automatically receive **live updates** on your EV charging status via:
- Push notifications to your mobile phone(s)
- Optional Text-to-Speech (TTS) announcements via your media players (e.g., Nest Hub, Alexa)
- Dynamic notification titles with ⚡ (charging) or ✅ (fully charged)
- Auto-clearing of notifications once unplugged
- Supports unit preference for Miles or Kilometers

---

[![Import Blueprint](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?url=https://raw.githubusercontent.com/Beel12213/ev-charging-notification/main/ev_charging_notification.yaml)

---

## ✨ Features

- 📱 Sends push notifications to multiple selected mobile devices
- 🎙️ Announces charging updates via selected media players using TTS
- 🔔 Persistent sticky notification inside Home Assistant UI
- 🔁 Live updates every 2 minutes or on sensor changes
- ✅ Auto-dismiss notifications when charger unplugged
- 🛞 Distance units selectable between Miles or Kilometers
- 🔥 Dynamic notification titles with icons (⚡ Charging / ✅ Fully Charged)

---

## 📋 Requirements

- Home Assistant
- Home Assistant Mobile App (for mobile push)
- One or more media_player devices (for optional TTS)
- Sensors providing:
  - Charger Connection Status (Connected/Disconnected)
  - Charging Power (in Watts)
  - Battery Level (%)
  - Estimated Finish Time
  - Estimated Range (km)

---

## 🛠️ Setup

1. Click the **Import Blueprint** button above ☝️
2. Create a new Automation using this Blueprint.
3. Fill in the required fields:
    - Select your charger sensors.
    - Pick your mobile device(s) for push notifications.
    - (Optional) Pick your media_player(s) for TTS announcements.
    - Choose your preferred distance unit (Miles or Kilometers).
4. Save and enable the automation. 🚀

---

## 📸 Example Notifications

**While Charging:**
> ⚡ Charging: 6.9kW at 45%  
> Estimated to finish at 03:30

**When Fully Charged:**
> ✅ Fully Charged: 80%  
> Estimated available range: 280 miles

## 🚀 Future Ideas

- Critical notification if charging unexpectedly stops
- Cost estimation based on energy usage
- Charge session statistics tracking
