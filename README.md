# Vedic Birth-Chart

A simple command-line tool that:

1. Computes your birth-chart (planetary longitudes + Ascendant) using [Swiss Ephemeris](https://www.astro.com/swisseph/).  
2. Formats each planet’s position as **Sign** + **°′** (e.g. `Sun  Sagittarius 13°00′`).  
3. Runs a local `interpret_chart()` routine to give quick Sun–Moon–Mars… readings.  
4. Sends a summary to TinyLlama for **12-month predictions** and **remedial measures**, printing everything to the console.  
5. (Optionally) Plots a polar “zodiac wheel” with your planets marked.

---

## 🔑 Features

- **Interactive CLI**: prompts you for DOB, time, place, and name.
- **Geocoding** via OpenStreetMap/Nominatim.
- **Accurate ephemeris**: uses Swiss Ephemeris for modern planetary positions.
- **Local interpretations**: built-in Vedic quick reads for each planet.
- **TinyLlama integration**: detailed monthly forecasts & remedies.
- **Console-only output**: no files or PDFs—just clean, immediate feedback.
- **Optional chart**: a polar-plot wheel of your birth chart.

---

## ⚙️ Prerequisites

- **Python 3.8+**  
- [Swiss Ephemeris](https://www.astro.com/swisseph/) data files (download and unpack)  
- A running [Ollama](https://ollama.com/) server with the `tinyllama` model installed  

---

### Chart Wheel

![Birth Chart Wheel](output.png)

### Planetary Positions

| Planet  | Sign         | Degrees  |
| ------- | ------------ | -------- |
| Sun     | Aquarius     | 10°17′   |
| Moon    | Aquarius     | 06°23′   |
| Mars    | Leo          | 27°39′   |
| Mercury | Aquarius     | 19°17′   |
| Jupiter | Sagittarius  | 10°07′   |
| Venus   | Sagittarius  | 24°14′   |
| Saturn  | Pisces       | 10°55′   |
| Rahu    | Scorpio      | 10°12′   |
| Ketu    | Taurus       | 10°12′   |

---

## 🔧 Installation

1. **Clone** this repo:  
   ```bash
   git clone https://github.com/<your-username>/vedic-birth-chart-cli.git
   cd vedic-birth-chart-cli
