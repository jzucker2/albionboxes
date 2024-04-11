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
* https://www.youtube.com/watch?v=0t12tRsphlM
* https://community.home-assistant.io/t/what-is-dashboard-import/422519/4

## Resources

* https://esphome.io/guides/faq
* https://esphome.io/guides/getting_started_hassio
