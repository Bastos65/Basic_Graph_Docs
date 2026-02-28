# BASIC GRAPH - Complete Documentation

> ⚠️ **DISCLAIMER**: This repository contains user documentation only. No source code, algorithms, backend logic or licensing mechanisms are included. Any attempt to reverse engineer the product is prohibited.

![Version](https://img.shields.io/badge/version-1.0.0-blue)
![Platform](https://img.shields.io/badge/platform-Garmin%20Connect%20IQ-green)
![API](https://img.shields.io/badge/API-5.0.0%2B-orange)

---

## Table of Contents

1. [Overview](#overview)
2. [Main Features](#main-features)
3. [User Interface](#user-interface)
4. [Configuration](#configuration)
   - [System Settings](#system-settings)
   - [Display Settings](#display-settings)
   - [Data Fields](#data-fields)
   - [Graph Field](#graph-field)
   - [Color Customization](#color-customization)
   - [Weather](#weather)
5. [Available Data Types](#available-data-types)
6. [Glossary](#glossary)
7. [Appendices](#appendices)

---

![BASIC GRAPH Banner](docs/images/Banner.jpg)

---

## Overview

**BASIC GRAPH** is a clean and data-rich watch face for Garmin Connect IQ watches. Built around a central graph field displaying historical data, it combines 6 circular fields, classic top data fields, and extensive customization to give maximum information at a glance.

### Key Features

- 📊 **Central Graph Field**: Line or Bar graph with up to 4 hours of history
- 🔵 **6 Circular Data Fields**: Positioned at 1h, 3h, 5h, 7h, 9h, 11h
- 📋 **3 Classic Top Fields**: Left, Center, Right configurable fields
- 🎨 **22 Customizable Colors**: Complete color control
- 🌦️ **Weather Integration**: Garmin Weather and OpenWeatherMap
- ⚡ **Battery Optimization**: Intelligent power saving modes
- 🌍 **Multilingual Support**: 19 languages available
- 🎯 **Goal Ring**: Visual goal progress tracking

---

## Main Features

### 1. Time Display

- 12h or 24h format
- Seconds display (3 modes: Hidden, Normal, Always On)
- Optional leading zero for hours
- AM/PM support in 12h format
- Independent colors for hours, minutes, seconds, separator

### 2. Graph Field

The central feature of BASIC GRAPH — a configurable graph displaying time-series data:

- **Line Graph**: Smooth line representation
- **Bar Graph**: Vertical bar representation
- **Duration**: 1 to 4 hours of history (for non-7-day data)
- **7 Days Mode**: Displays 7-day history with optional day letters
- **Goal line**: Optional display of the goal value
- **Custom goal**: Override the system goal with a custom value

### 3. Circular Data Fields

Six circular data fields positioned at clock positions 1h, 3h, 5h, 7h, 9h, 11h:

- Value display
- Customizable title
- Unit display
- Multiple display modes
- Independent color configuration

### 4. Classic Top Data Fields

Three data fields at the top of the watch face:

- Top Left field
- Top Center field
- Top Right field
- Colored icons (filled or outlined set)
- Text values

### 5. Top Text Field

- Fully configurable data type
- Multiple display modes (value, title+value, goal, etc.)
- Customizable title

### 6. Info Indicators

Four visual indicators:

1. **Info 1**: Configurable indicator
2. **Info 2**: Configurable indicator
3. **Info 3**: Configurable indicator
4. **Info 4**: Configurable indicator

### 7. Goal Ring

- Graphical progress visualization
- Multiple goal data types
- Configurable range (min/max)

### 8. Date

- 7 display formats
- Day of the week
- International format support

### 9. Weather

- **Sources**: Garmin Weather and/or OpenWeatherMap
- **Available Data**:
  - Current, feels like, min/max temperature
  - Weather description and icon
  - Humidity
  - Wind speed and direction
  - Atmospheric pressure (OWM)
  - Cloud coverage (OWM)
  - Visibility (OWM)
  - Precipitation probability (GW)

---

## User Interface

### Screen Structure

![Watch Face Layout](docs/images/Display_Overview.png)

*BASIC GRAPH display layout showing all configurable zones*

### Display Modes

#### Full Display Mode
![Full Display](docs/images/Display_1.png)

#### Screen Saver Mode
![Screen Saver](docs/images/Layout_Screen_Saver.png)

### Legend
- **Time**: Time display
- **Date**: Date display
- **Graph**: Central graph field
- **Circ 1h/3h/5h/7h/9h/11h**: Circular fields
- **TL/TC/TR**: Top fields (Left/Center/Right)
- **I1/I2/I3/I4**: Information indicators
- **Goal Ring**: Goal progress ring

---

## Configuration

### System Settings

#### Data Refresh Rate
Controls data update frequency:

- **Full Refresh**: Complete update every second (maximum consumption)
- **High Refresh Rate**: High refresh
- **Medium Refresh Rate**: Medium refresh (recommended)
- **Low Refresh Rate**: Low refresh (battery saving)

#### Power Saving

**Screen Saver Delay**: Delay in minutes before screen saver activation (-1 to disable)

**Screen Off Delay**: Delay in minutes before screen turns off (-1 to disable)

#### Widget

**Launch Widget On Press Hold**: Launch widget on long press (touchscreen only)

---

### Display Settings

#### Time Format

**Use Military Format**:
- `true`: 24-hour format
- `false`: 12-hour format (AM/PM)

**Hours Leading 0**:
- `true`: Display leading zero (01, 02, 03...)
- `false`: No leading zero (1, 2, 3...)

**Seconds Display Mode**:
1. **Hidden**: Seconds hidden
2. **Normal**: Normal seconds display
3. **Always On**: Always displayed

#### Date Format

7 available display modes:

1. `[DOW dd Month]`: Mon 15 January
2. `[DOW dd/mm]`: Mon 15/01
3. `[dd/mm/yyyy]`: 15/01/2026
4. `[DOW Month dd]`: Mon January 15
5. `[Month dd DOW]`: January 15 Mon
6. `[DOW mm/dd]`: Mon 01/15
7. `[yyyy/mm/dd]`: 2026/01/15

---

### Data Fields

#### Configuration for Each Field

For each data field, you can configure:

1. **Data Type**: Choose from 73+ types (see Data Types section)
2. **Custom Title**: Free text to replace default title
3. **Display Mode**: How to display the data

#### Display Modes

##### Circular Fields (1h, 3h, 5h, 7h, 9h, 11h)

0. **Value**: Value only
1. **Title + Value**: Title above value
2. **Value + Unit**: Value with unit
3. **Value + Title**: Value with title below
4. **Title Value Unit**: Title, value, unit

##### Top Text Field

0. **Value**: Value only
1. **Title + Value**: Title and value
2. **Value + Unit**: Value with unit
3. **Value + Title**: Value with title
4. **Title Value Unit**: Title, value, unit
5. **Title**: Title only
6. **Goal**: Goal display
7. **Value / Goal**: Value over goal
8. **Percents Of Goal**: Goal percentage
9. **Remaining**: Remaining to reach goal

---

### Graph Field

The graph field is the central element of BASIC GRAPH.

#### Graph Data Type

Select the data type to display in the graph from all available data types.

#### Graph Display Mode

- **Line Graph**: Smooth line chart
- **Bar Graph**: Vertical bar chart

#### Graph Duration

For non-7-day data types: duration in hours (1 to 4 hours).

#### 7 Days Options

- **Display 7 Days Graph Day Letters**: Show abbreviated day names below bars
- **Display Graph Goal**: Show a horizontal goal line on the graph

#### Goal Configuration

- **Display Graph Goal**: Toggle goal line visibility
- **Custom Graph Field Goal**: Override system goal value (0 = use system goal)

---

### Color Customization

BASIC GRAPH offers **22 customizable colors**:

| ID | Element |
|----|---------|
| 0 | Background Color |
| 1 | Separation Lines Color |
| 2 | Circular Fields Title/Unit Text Color |
| 3 | Circular Fields Value Text Color |
| 4 | Text Fields Text Color |
| 5 | Data Fields Value Color |
| 6 | Data Field Top Left Title/Icon Color |
| 7 | Data Field Top Center Title/Icon Color |
| 8 | Data Field Top Right Title/Icon Color |
| 9 | Time Hours Color |
| 10 | Time Sep Color (separator) |
| 11 | Time Minutes Color |
| 12 | Time Seconds & AM/PM Color |
| 13 | Graph Field Value Color |
| 14 | Graph Field Goal Color |
| 15 | Info Off Color |
| 16 | Info 1 On Color |
| 17 | Info 2 On Color |
| 18 | Info 3 On Color |
| 19 | Info 4 On Color |
| 20 | Goal Ring Off Color |
| 21 | Goal Ring On Color |

### Predefined Color Palette

The watch face offers **67 predefined colors** organized by family.

➡️ **[View complete color list](https://pay.b65dev.com/portfolio/faqs#faq-colors)**

### Special Color Options

**Use Battery Adaptative Color**: Automatically adapts color based on battery level

**Use Weather Colored Icons**: Colors weather icons according to conditions

**Custom Colors**: Define up to 3 custom colors via hexadecimal code (format: `0xffffff` or `ffffff`)

---

### Weather

#### Provider Configuration

**Weather Provider**: Weather service selection

1. **Garmin Weather (GW)**: Native Garmin service
2. **OpenWeatherMap (OWM)**: External service requiring API key
3. **Garmin Weather + OpenWeatherMap**: Garmin priority, OWM complement
4. **OpenWeatherMap + Garmin Weather**: OWM priority, Garmin complement

#### OpenWeatherMap

**Weather Key**: OpenWeatherMap API key (32 characters max)

To obtain an API key:
1. Create an account on [openweathermap.org](https://openweathermap.org)
2. Generate a free API key
3. Copy the key into the settings

**Weather Call**: Displays last API call time (read-only)

---

### Units of Measurement

#### Altitude
- Meters (m)
- Feet (ft)

#### Distance
- Kilometers (km)
- Miles (mi)
- International Nautical Miles (nm)

#### Temperature
- Celsius (°C)
- Fahrenheit (°F)
- Kelvin (°K)

**Temperature Offset**: Temperature sensor correction (numeric value)

#### Pressure
- Hectopascal (hPa)
- Millimeters Of Mercury 0°C (mmHg)
- Inch Of Mercury 0°C (inHg)

#### Weight
- Kilograms (kg)
- Pounds (lbs)

#### Wind Speed
- Meters / Seconds (m/s)
- Kilometers / Hours (km/h)
- Miles / Hours (mi/h)
- Knots (kn)
- Beaufort Scale (bf)

#### Wind Direction
- **Degrees Direction**: Degree display (000-360)
- **Cardinal Direction**: Cardinal display (N, NE, E, SE, S, SW, W, NW)

---

### Advanced Settings

#### Custom Texts

**Custom Text 1 Value**: Free text for custom display  
**Custom Text 2 Value**: Second free text

#### Countdown

**Countdown Target Day**: Countdown target date  
**Countdown Target Hour**: Target time (format HH:mm:ss, e.g.: 14:30:00)

#### Time Zones

Configuration of 4 additional time zones:

- **Time Zone 2**: UTC format (e.g.: +02:00 or -05:30)
- **Time Zone 3**: UTC format
- **Time Zone 4**: UTC format
- **Time Zone 5**: UTC format

Format: HH:mm with + or - sign (e.g.: `+02:00`, `-05:30`)

#### Icon Sets

**Icons Set**:
- **Filled Icons**: Solid icons
- **Outlined Icons**: Outlined icons

---

## Available Data Types

BASIC GRAPH supports **73+ different data types**. Here is the complete list:

### Physical Activity

| Type | Description |
|------|-------------|
| Active Minutes : Daily | Daily active minutes |
| Active Minutes : Weekly | Weekly active minutes |
| Calories : Daily Burned | Daily burned calories |
| Calories : Daily Burned Active | Active burned calories |
| Steps Daily | Daily step count |
| Distance : Daily | Today's distance |
| Distance : Weekly | This week's distance |
| Floors Climbed : Daily | Today's climbed floors (if available) |

### Specific Distances

| Type | Description |
|------|-------------|
| Bike Distance : Week | Week's cycling distance |
| Bike Distance : 30 Days | 30-day cycling distance |
| Bike Distance : Current Month | Current month's cycling distance |
| Run Distance : Week | Week's running distance |
| Run Distance : 30 Days | 30-day running distance |
| Run Distance : Current Month | Current month's running distance |
| Pushes | Number of pushes (if available) |
| Pushes Distance Daily | Daily push distance (if available) |

### Health and Wellness

| Type | Description |
|------|-------------|
| Heart Rate | Current heart rate |
| Heart Rate Min/Max (4 Hours) | HR min/max over 4 hours |
| Body Battery | Body battery level (if available) |
| Stress Level | Stress level (if available) |
| Respiration Rate | Respiration rate (if available) |
| Oxygen Saturation | Oxygen saturation / SpO2 (if available) |
| Recovery Time | Recovery time in hh:mm (if available) |
| Weight | Weight in kg |

### Sports Performance

| Type | Description |
|------|-------------|
| VO2 Max Cycling | Cycling VO2 Max (if available) |
| VO2 Max Running | Running VO2 Max (if available) |
| Race Predictor 5K | 5K time prediction |
| Race Predictor 10K | 10K time prediction |
| Race Predictor Half Marathon | Half marathon prediction |
| Race Predictor Marathon | Marathon prediction |
| Training Status | Training status |

### System and Battery

| Type | Description |
|------|-------------|
| Battery In Days | Battery life in days |
| Battery In Percents | Battery level in % |
| Solar Intensity | Solar intensity (if available) |
| Phone Connected | Phone connected |
| Alarms Count | Number of alarms |
| Notifications Count | Number of notifications |
| Move Alert Level | Move alert level |
| Do Not Disturb Enabled | Do not disturb enabled |

### Environment

| Type | Description |
|------|-------------|
| Altitude | Current altitude (if available) |
| Pressure From Sensor | Atmospheric pressure (if available) |
| Temperature From Sensor | Sensor temperature (if available) |

### Weather (Garmin Weather)

| Type | Description |
|------|-------------|
| Weather Description | Weather description |
| Weather Temperature | Weather temperature |
| Weather Temperature : Feel | Feels like temperature |
| Weather Temperature : Min / Max | Min/max temperatures (GW only) |
| Weather Humidity | Humidity |
| Weather Precipitation Probability | Precipitation probability (GW only) |
| Weather Wind Speed/Direction | Wind speed and direction |
| Weather GW Update Time | Garmin Weather update time |

### Weather (OpenWeatherMap)

| Type | Description |
|------|-------------|
| Weather Station | Weather station (OWM only) |
| Weather Clouds Cover | Cloud coverage (OWM only) |
| Weather Pressure | Pressure (OWM only) |
| Weather Visibility | Visibility (OWM only) |
| Weather OWM Update Time | OpenWeatherMap update time |

### Sun and Moon

| Type | Description |
|------|-------------|
| Sun Event : Daily Sunrise | Sunrise |
| Sun Event : Daily Sunset | Sunset |
| Sun Event : Next Sun Event | Next sun event |
| Sun Event : Civil Dawn | Civil dawn |
| Sun Event : Civil Dusk | Civil dusk |
| Moon Age | Moon age |
| Moon Illumination | Moon illumination |
| Moon Phase | Moon phase |

### Date and Time

| Type | Description |
|------|-------------|
| Date | Current date |
| Day Of The Year | Day of the year |
| Week Of The Year | Week of the year |
| Time Zone 2 | Time zone 2 |
| Time Zone 3 | Time zone 3 |
| Time Zone 4 | Time zone 4 |
| Time Zone 5 | Time zone 5 |
| Countdown | Countdown |

### Customization

| Type | Description |
|------|-------------|
| Custom Text | Custom text 1 |
| Custom Text 2 | Custom text 2 |
| Hidden Field | Hidden field |

### Debug

| Type | Description |
|------|-------------|
| Debug Data | Debug data |

---

## Glossary

- **AMOLED**: Active Matrix Organic Light-Emitting Diode display type
- **API**: Application Programming Interface
- **Connect IQ**: Garmin platform for third-party applications
- **GW**: Garmin Weather (Garmin weather service)
- **OWM**: OpenWeatherMap (external weather service)
- **SpO2**: Pulse oxygen saturation
- **VO2 Max**: Maximum oxygen consumption
- **UTC**: Coordinated Universal Time

---

## Appendices

### Parameter Formats

#### Custom Colors
Hexadecimal format: `0xRRGGBB` or `RRGGBB`
- RR = Red (00-FF)
- GG = Green (00-FF)
- BB = Blue (00-FF)

Example: `0xFF0000` = Pure red

#### Time Zones
Format: `±HH:mm`
- + sign for East, - for West
- HH = Hours (00-14)
- mm = Minutes (00 or 30)

Examples:
- `+01:00` = UTC+1 (Paris)
- `-05:00` = UTC-5 (New York)
- `+05:30` = UTC+5:30 (India)

#### Countdown Hour
Format: `HH:mm:ss`
- HH = Hours (00-23)
- mm = Minutes (00-59)
- ss = Seconds (00-59)

Example: `14:30:00` = 2:30 PM

### Moon Phase Codes

Moon phases are numbered from 0 to 7:
- 0: New Moon
- 1: Waxing Crescent
- 2: First Quarter
- 3: Waxing Gibbous
- 4: Full Moon
- 5: Waning Gibbous
- 6: Last Quarter
- 7: Waning Crescent

---

**Last updated**: February 28, 2026  
**Document version**: 1.0  
**Author**: Bastos65

---

*This document is provided "as is" without warranty of any kind. The developer reserves the right to modify features and documentation without notice.*
