# ESP32 Temperature and Humidity Monitoring Using ThingSpeak

## Student Information

- **Name:** Dana Morgan
- **University ID:** 12218098

## Project Description

This project uses an ESP32 and a DHT22 sensor to monitor temperature and humidity using the Wokwi simulator.

The ESP32 connects to Wi-Fi and sends the readings to ThingSpeak every 20 seconds. The data is displayed on two separate charts to monitor temperature and humidity changes over time.

## Components Used

- ESP32 Development Board
- DHT22 Temperature and Humidity Sensor
- LED and Resistor
- Breadboard
- Wokwi Simulator
- ThingSpeak Platform

## Wiring Connections

| Component  | ESP32 Connection        |
| ---------- | ----------------------- |
| DHT22 VCC  | 3.3V                    |
| DHT22 GND  | GND                     |
| DHT22 DATA | GPIO 15                 |
| LED        | GPIO 23 (with resistor) |

The LED turns on when the temperature exceeds 30°C.

## ThingSpeak Channel

- **Channel Name:** Dana_Morgan_12218098
- **Channel ID:** 3551742
- **Field 1:** Temperature (°C)
- **Field 2:** Humidity (%)
- **Access:** Public

**Public Channel URL:**

[https://thingspeak.com/channels/3551742](https://thingspeak.com/channels/3551742)

## Wokwi Simulation

**Wokwi Project Link:**

[https://wokwi.com/projects/479319347109539841](https://wokwi.com/projects/479319347109539841)

## How It Works

1. The ESP32 connects to the Wokwi Wi-Fi network.
2. The DHT22 sensor measures temperature and humidity.
3. The readings are displayed in the Serial Monitor along with the university ID.
4. The ESP32 sends both values to ThingSpeak every 20 seconds.
5. ThingSpeak displays the readings on separate temperature and humidity charts.
6. The LED turns on when the temperature is above 30°C.

## Results and Visualization

The ESP32 successfully connected to Wi-Fi and sent temperature and humidity readings to ThingSpeak.

Both charts show the changes in temperature and humidity over time.

**Note about the charts:**

The ThingSpeak channel was created three days before the final test, so it already contained readings from earlier experiments.

To make the latest results easier to see, I configured both charts to display only the **last 7 readings** instead of showing all historical data.

This makes the recent temperature and humidity changes clearer and keeps the timeline focused on the final test. The older readings are still stored in the ThingSpeak channel.

## Screenshots

The `screenshots` folder includes:

- `wokwi-circuit` — ESP32 circuit and wiring diagram.
- `serial-monitor` — Sensor readings and successful data transmission.
- `thingspeak-channel` — Public ThingSpeak channel information.
- `temperature-graph` — Temperature readings over time.
- `humidity-graph` — Humidity readings over time.
- `thingspeak-results` — Both ThingSpeak charts together.

## Running the Project

1. Open the Wokwi project.
2. Add your own ThingSpeak Write API Key to the source code.
3. Start the simulation.
4. Check the Serial Monitor for the sensor readings.
5. Open the public ThingSpeak channel to view the updated charts.

**Note:** The Write API Key is not included in the public GitHub source code for security reasons.
