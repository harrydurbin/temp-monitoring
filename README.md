## IoT Home Temperature Monitoring System

To monitor indoor temperature I set up a Raspberry Pi connected to an Adafruit DS18B20 temperature sensor. Instructions for configuring the sensor are found in the sensor guidelines: https://learn.adafruit.com/adafruits-raspberry-pi-lesson-11-ds18b20-temperature-sensing/hardware. <br/>

In addition indoor temperature, outdoor temperature readings are collected through the wunderground weather API. An Auto-Regressive Integrated Moving Average (ARIMA) model is used to make upcoming forecastes. <br/>

To store data, a SQLite database is used to collect hourly readings. The data is added online to Plolty to stream data stream in real-time: https://plot.ly/~harry.durbin/80.embed

![alttag](https://github.com/harrydurbin/temperature-monitoring/blob/master/img/stream.png)
