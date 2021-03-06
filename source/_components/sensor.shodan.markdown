---
layout: page
title: "Shodan Sensor"
description: "Instructions how to integrate Shodan sensors into Home Assistant."
date: 2017-08-09 10:30
sidebar: true
comments: false
sharing: true
footer: true
ha_category: Sensor
ha_iot_class: "Cloud Polling"
logo: shodan.png
ha_release: 0.51
---


The `shodan` sensor platform is displaying the total of result of a [Shodan](https://pi-hole.net/) query.

Use "Show API Key" in the upper right corner when you are logged in or got to your "My Account" page to retrieve your API key.

To enable this sensor, add the following lines to your `configuration.yaml` file for a GET request:

```yaml
# Example configuration.yaml entry
sensor:
  - platform: shodan
    api_key: SHODAN_API_KEY
    query: 'home-assistant'
```

Configuration variables:

- **api_key** (*Required*): The API key for Shodan.io.
- **query** (*Required*): The search string.
- **name** (*Optional*): Name of the Shodan sensor.

