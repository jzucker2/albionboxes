# ESPHome

This is just a basic landing page for the ESPHome stuff, which has really taken over this repo.

## Updating

```
pip install --upgrade -r upgrade-requirements.txt
```

* https://esphome.io/components/display/index.html
  * This has info about the `Pillow` version

## Naming

* https://community.home-assistant.io/t/entity-name-as-just-friendly-name/616835/15

### Issues with `friendly_name`

* https://github.com/esphome/feature-requests/issues/2476
* https://community.home-assistant.io/t/how-is-friendly-name-supposed-to-behave/542570/9

Turns out that it will shove `friendly_name` in front of an 
entity, _even_ if that entity is already prepended with the 
expanded `${friendly_name}`. This causes it to double so that 
it reads as `Dan Desk Temp Sensor Dan Desk Temp Sensor Uptime Sensor` 
instead of just simply `Dan Desk Temp Sensor Uptime Sensor`.

## Dashboard Import

* https://esphome.io/guides/creators.html
* https://esphome.io/guides/configuration-types#config-git-packages
* https://www.youtube.com/watch?v=0t12tRsphlM
* https://community.home-assistant.io/t/what-is-dashboard-import/422519/4

## Framework: Arduino vs. ESP-IDF

* Explains the difference between the 2 frameworks
  * https://github.com/mmakaay/esphome-xiaomi_bslamp2/issues/62
* Docs for setting the 2 possibilities
  * https://esphome.io/components/esp32.html
* Recommended versions of both frameworks in the code
  * https://github.com/esphome/esphome/blob/76daefe21c5f7a405d3f7df232bb7df0a2f4fe09/esphome/components/esp32/__init__.py#L229

## Issues

* Ghost button presses
  * https://community.home-assistant.io/t/atom-lite-rgb-led-turns-on-by-itself/452852/11
  * https://community.m5stack.com/topic/3955/atom-button-at-gpio39-without-pullup/11
* Internal temp issues
  * https://github.com/esphome/issues/issues/4271
  * https://github.com/espressif/esp-idf/issues/8088
* M5Stack PoE W5500 chip has issues with ESPHome
  * https://github.com/esphome/esphome/pull/7503
* LoRa M5Stack support
  * https://github.com/esphome/esphome/pull/7490

## Concepts

* substituting text strings in C++
  * https://esphome.io/components/display/#display-printf
* update numeric values from text in a lambda
  * https://esphome.io/cookbook/lambda_magic.html#update-numeric-values-from-text-input
  * TODO: add a conversion to the version text label to output to a gauge sensor for prometheus
* other lambda helper functions
  * https://github.com/esphome/esphome/blob/dev/esphome/core/helpers.h
  * Hex conversion and printing
    * https://community.home-assistant.io/t/hex-string-to-dec-value/458945/9
    * https://github.com/esphome/esphome/blob/dev/esphome/components/ble_client/sensor/ble_sensor.cpp
* Functions and import stuff
  * https://community.home-assistant.io/t/reusable-function-for-lambdas/296435/9

## General Resources

* https://esphome.io/guides/faq
* https://esphome.io/guides/getting_started_hassio
* https://esphome.io/guides/getting_started_command_line
* https://esphome.io/guides/configuration-types
* https://esphome.io/guides/creators.html
* https://esphome.io/components/external_components
* https://esphome.io/components/esp32.html
* https://esphome.io/components/esphome
* https://github.com/Chill-Division/M5Stack-ESPHome
* https://github.com/SmartHome-yourself/m5-dial-for-esphome
  * M5 Dial project
* https://community.home-assistant.io/t/m5stack-dial-esp32-s3-smart-rotary-knob/623518/98
  * Best M5 Dial project and notes so far
  * https://www.thingiverse.com/thing:6477677
