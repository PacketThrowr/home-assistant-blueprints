# 🎬 Hassarr Downloads – Home Assistant Blueprints

A collection of Home Assistant blueprints that use **Hassarr** to request and download movies or TV shows from **Overseerr**, **Sonarr**, or **Radarr** via any LLM-enabled voice assistant (Assist, OpenAI, etc.).

These blueprints create scripts that your LLM calls whenever a user says:

- “Download the movie *Inception*.”
- “Add the TV show *Severance*.”
- “Grab *Interstellar* for me.”

The script extracts the title → sends it to Hassarr → Overseerr/Sonarr/Radarr handles the download.

---

## 📦 Prerequisites

Before installing the blueprint, make sure you have:

1. **Overseerr OR Sonarr/Radarr installed and running**
2. The custom integration **[Hassarr](https://github.com/TegridyTate/Hassarr)** installed  
   *(HUGE thanks to **TegridyTate** for creating this integration!)*
3. **Restart Home Assistant** after installing Hassarr
4. Configure Hassarr:  
   `Settings → Devices & Services → Integrations → Add → Hassarr`  
   Add Overseerr or Radarr/Sonarr with their API keys
5. A **conversation agent connected to an LLM**  
   (Assist + OpenAI, Home Assistant Cloud, etc.)

---

## 📥 Installation

Click the button below to import the blueprint into Home Assistant:

### 📘 Overseerr Blueprint

| Blueprint | Description | Link |
|-----------|-------------|------|
| `overseerr-downloads.yaml` | Uses Overseerr via Hassarr to request TV shows or movies | [![Open your Home Assistant instance and show the blueprint import dialog with a specific blueprint pre-filled.](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A%2F%2Fgithub.com%2FPacketThrowr%2Fhome-assistant-blueprints%2Fblob%2Fmain%2Fhassarr-downloads%2Foverseerr-downloads.yaml) |

---

## 🛠️ Setup Steps

1. **Click the import button above**
2. Home Assistant will show the *Create Script* dialog  
   → Click **Save**
3. Open your new script  
   → **Expose it to Assist**
4. Done! 🎉

Your assistant can now use this script as a tool.

---

## 🎤 How to Use

Just speak naturally to your voice assistant:

- **“Download the movie Superman.”**
- **“Add the TV show Arcane to Overseerr.”**
- **“Request Dune Part Two.”**
- **“Grab the show Fallout.”**

Your LLM parses:

- `media_type` (movie/tv)
- `title`

…and the blueprint sends it directly to Hassarr for processing.

---

## 🤝 Credits

- **Hassarr Integration:**  
  https://github.com/TegridyTate/Hassarr  
  Maintained by **TegridyTate** — amazing work!

- Blueprint designed and maintained by **PacketThrowr**

---

## 📝 License

This project is released under the MIT license.  
Feel free to fork, modify, and contribute!
