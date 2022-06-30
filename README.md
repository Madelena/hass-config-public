# My Home Assistant Config

## Maximalist Dashboard

This is a redacted version of my personal dashboard configuration for [Home Assistant](https://www.home-assistant.io/), an open source home automation server that integrates nearly 2000 existing IoT services into one powerful, private, and unified user interface.

[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/madelena)

**✨ Thank you @legovaer and @pbohannon for your generous support! ✨**

## Table of Contents

- [Design Principles](#design-principles)
- [Screenshots Tour ↗](https://github.com/Madelena/hass-config-public/wiki/Views-and-Cards)
- [Features](#features)
- [How to Install](#how-to-install)
- [Specifications ↗](https://github.com/Madelena/hass-config-public/wiki/Specifications) - Hardware, Ecosystem, List of Integrations, etc.
- [Tools Used](#tools-used)
- [Credits](#credits)

## Design Principles

The design is based on the principle that *data is beautiful*.

Contrary to conventional UX design, the dashboard is intentionally dense with information and not minimalist, because it is designed for only one power user: me.

My goal is to create a sense of awareness of my surroundings and my resources through information, while my second priority is to be able to control and fine-tune all aspects of my living space. This is not designed for convenience since I already have physical buttons and switches for such purpose.

![HA Config - Summary](https://user-images.githubusercontent.com/4341881/173772319-907d6821-b96c-4d07-96d0-c0fd02efe2b6.png)

The dashboard is designed to maximize the amount of information displayed without additional user interactions, acting as an ambient display in the background. Information is not hidden or tucked away from view but is instead shown in its full glory for those who love to look at real-time data visualizations.

Animation is toned down so that it still feels responsive but not distracting. Colors are used to draw attention to things that I need to attend to, and the monochromatic color scheme keeps the visual priority clear. The wireframe aesthetic for illustrations and flat icons keeps visual noise to the minimum.

It uses my own [Metrology theme](https://github.com/Madelena/Metrology-for-Hass), based on Metro design system, to reduce visual clutter, create a sense of visual hierarchy, and focus on the data.

[View all the dashboards here.](https://github.com/Madelena/hass-config-public/wiki/Views-and-Cards)

## Features

### Data Visualizations - Make it Beautiful
Data is beautiful! Data in HA is used to render some unique, eye-catching, and informative graphs as the visual focus of each page.

<table>
  <tr>
    <td width="33%" valign="bottom">
<img alt="HA Dataviz - Axonometric Floor Plan" src="https://user-images.githubusercontent.com/4341881/176595331-a6edadef-ab2c-4927-8c9c-3bbbc1fed213.png"><br/>
Axonometric Floor Plan</td>
    <td width="33%" valign="bottom">
<img width="50%" alt="HA Dataviz - Network Map" src="https://user-images.githubusercontent.com/4341881/176595345-7267d37c-d119-444f-a676-620b132809e5.png"/><br/>
Network Rail Map</td>
    <td width="33%" valign="bottom">
<img alt="HA Dataviz - Energy Sankey" src="https://user-images.githubusercontent.com/4341881/176595367-89c1a694-3270-43ab-80f8-f55119be2910.png"/><br/>
Energy Use Sankey Diagram</td>
  </tr>
  <tr>
    <td width="33%" valign="bottom">
<img alt="HA Dataviz - Psychrometry Chart" src="https://user-images.githubusercontent.com/4341881/176595376-7f409b71-404b-4d68-afa7-230e5d85eeec.png"/><br/>
Psychrometry Chart</td>
    <td width="33%" valign="bottom">
<img alt="HA Dataviz - Weather History" src="https://user-images.githubusercontent.com/4341881/176595385-9955e68e-c1f5-4334-98fa-88d425236789.png"/><br/>
Weather History + Forecast Chart</td>
    <td width="33%" valign="bottom"><img alt="Music Chart" src="https://user-images.githubusercontent.com/4341881/173772638-4140700a-31e6-4c26-821a-2ef0ba24d9c1.jpeg"/><br/>Last.fm Music Charts</td>
  </tr>
</table>

All visualizations adhere to theme colors and light/dark modes.

Additional visualizations are embedded from third-party sources.

<table>
  <tr>
    <td width="33%" valign="bottom">
<img src="https://user-images.githubusercontent.com/4341881/176596390-b87e65a5-bee1-4e0d-857e-af085329a067.png"><br/>
The Weekendest Subway Map</td>
    <td width="33%" valign="bottom">
<img src="https://user-images.githubusercontent.com/4341881/176596167-19c31668-02e6-47f6-908a-ee9f9da357b6.png"/><br/>
Bing Traffic Static Map</td>
    <td width="33%" valign="bottom"><img src="http://s.w-x.co/staticmaps/wu/wu/wxtype1200_cur/usbgm/animate.png"/><br/>Weather Underground Radar Map</td>
  </tr>
  <tr>
    <td width="33%" valign="bottom">
<img src="https://user-images.githubusercontent.com/4341881/176596556-c96f476b-b750-4d4b-a6a4-9360b1a09509.png"><br/>jsOrrery Solar System Map</td>
    <td width="33%" valign="bottom">
<img src="https://user-images.githubusercontent.com/4341881/176596708-ddd33534-d974-4f0e-97c9-c4b9138dd973.png"><br/>
Astropheric Weather Chart</td>
  </tr>
</table>


## How to install

The code is not meant to be installed as sensitive information had been redacted from the configuration. It is meant to be used as a reference to do some pretty wonderful things using lots of clever or ugly codes, tips, tricks, and hacks. Copy and paste stuff to your own dashboard config as you see fit.

A few requisities will help you use these codes:

### Major HACS frontend mods

- button-card
- card-mod
- layout-mod
- mini-graph-card
- apexcharts-card
- [View the full list](https://github.com/Madelena/hass-config-public/wiki/Specifications)

### Template libraries

Include these lines in your dashboard YAML to use most of the templates defined in the config:

```yaml
decluttering_templates: !include cards/decluttering_templates.yaml
button_card_templates: !include cards/button_card_templates.yaml
apexcharts_card_templates: !include cards/apexcharts_card_templates.yaml
```

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
