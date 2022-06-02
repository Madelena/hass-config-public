# My Home Assistant Config

## Maximalist Dashboard

[Home Assistant](https://www.home-assistant.io/) is an open source home automation server that integrates nearly 2000 existing IoT services into one powerful, private, and unified user interface.

This is a redacted version of the dashboard configuration for my personal instance of Home Assistant.

## Design Principles

The design is based on the principle that *data is beautiful*. The dashboard is information dense - it is designed to maximize the amount of information displayed without additional user interactions. Information is not hidden or tucked away from view, but is shown in its full glory for those who like to read data.

It uses Metro design system to reduce visual clutter, create a sense of visual hierarchy, and focus on the data.

This also acts as a demo and example of what the Metrology theme is capable of.

## Features

- Data Visualizations
  - Data is beautiful! Data in HA is used to render some unique, eyecatching, and informative graphs as the visual focus of each page.
- Responsive Design
  - Grid reflows depending on screen width and device type
- Live Tiles
  - Animated to display multiple pieces of information
  - Variations based on states
- Summary Sentences for NUI
  - Intelligible sentences composed by aggregating data for use on page summaries and voice assistants

## Views and Cards

### Main Dashboard
- Summary
  - USS Strawberry Fields
- Network
  - Network Rail Map
- Energy
  - Sankey Chart
- Light
- Maintenance
  - Chore List
- Environment
  - Psychrometry Chart
  - Climate + Forecast Chart
- Neighborhood
  - Transit
  - Traffic
  - Weather
- Me
  - Last.fm Music
- Astrometrics

### My Machines
- Unison
- Genesis
- Terpsichora
- Printers


## How to install

The code is not meant to be installed as sensitive information had been redacted from the configuration. It is meant to be used as a reference to do some pretty wonderful things using lots of clever or ugly codes, tips, tricks, and hacks. Copy and paste stuff to your own dashboard config as you see fit.

A few requisities will help you use these codes:

### Major HACS frontend mods

- button-card
- card-mod
- layout-mod
- mini-graph-card
- apexcharts-card

### Template libraries

Include these lines in your dashboard YAML to use most of the templates defined in the config:

```yaml
decluttering_templates: !include cards/decluttering_templates.yaml
button_card_templates: !include cards/button_card_templates.yaml
apexcharts_card_templates: !include cards/apexcharts_card_templates.yaml
```

## Hardware

- Raspberry Pi 4 - 4GB RAM
- Corsair 128GB SSD
- ConBee

## Tools Used

- Code Server Add-On for HA
- Visual Studio Code
  - Bookmarks extension
- Inkscape / Adobe Illustrator
- SketchUp
- [Psychometry Chart](https://drajmarsh.bitbucket.io/psychro-chart2d.html) by [Dr. Andrew J. Marsh](http://andrewmarsh.com/)

## Credits

![Creative Commons License](https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png)

This work is licensed under a [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](http://creativecommons.org/licenses/by-nc-sa/4.0/).

Additionally, I would appreciate proper credits back to me if redistributed or modified. That would help my livelihood since design is [my career](https://MadelenaMak.com).
