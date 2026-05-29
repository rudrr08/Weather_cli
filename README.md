# 🌤️ Weather CLI

> Termux + Python se banaya gaya Weather CLI Tool — by [rudrr08](https://github.com/rudrr08)

Apne terminal se kisi bhi city ka **current weather** aur **5-day forecast** dekho!

---

## 📦 Installation

### Step 1 — Clone karo
```bash
git clone https://github.com/rudrr08/weather-cli.git
cd weather-cli
```

### Step 2 — Dependencies install karo
```bash
pip install -r requirements.txt
```

### Step 3 — API Key lo
1. [openweathermap.org](https://openweathermap.org) pe free account banao
2. API key copy karo
3. Environment variable set karo:

```bash
export OPENWEATHER_API_KEY=teri_api_key_yahan
```

---

## 🚀 Usage

### Current Weather
```bash
python -m weather_app.cli now Mumbai
python -m weather_app.cli now "New Delhi"
```

### 5-Day Forecast
```bash
python -m weather_app.cli forecast Mumbai
python -m weather_app.cli forecast Chennai
```

### API Key directly dena ho toh
```bash
python -m weather_app.cli now Mumbai --api-key YOUR_KEY
```

---

## 📸 Output Example

```
===================================
📍  Mumbai, IN
===================================
🌤️   Haze
🌡️   Temperature : 32.0°C
🤔  Feels Like  : 38.0°C
💧  Humidity    : 78%
💨  Wind Speed  : 5.2 m/s
👁️   Visibility  : 5 km
===================================
```

---

## 📁 Project Structure

```
weather-cli/
├── weather_app/
│   ├── __init__.py      # Package info
│   ├── weather.py       # API logic
│   └── cli.py           # CLI commands (Click)
├── tests/
│   └── test_weather.py  # Basic tests
├── requirements.txt
├── setup.py
├── .env.example
├── .gitignore
└── README.md
```

---

## 🛠️ Tech Stack

| Tool | Kaam |
|------|------|
| Python 3 | Main language |
| Click | CLI framework |
| Requests | HTTP calls |
| OpenWeatherMap API | Weather data |

---

## 📱 Termux pe kaise chalayein?

```bash
pkg install python
pip install requests click
git clone https://github.com/rudrr08/weather-cli.git
cd weather-cli
export OPENWEATHER_API_KEY=teri_key
python -m weather_app.cli now Mumbai
```

---

## 📄 License

MIT License — freely use karo!

---

Made with ❤️ in Termux
