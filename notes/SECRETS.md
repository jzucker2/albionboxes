# Secrets

Create a file `albionboxes/secrets.yaml` (Note the _exact_ `.yaml` filename extension) with the following:

```yaml
# https://esphome.io/components/wifi.html
wifi_ssid: My Wifi Network
wifi_password: supersecretpassword
# https://esphome.io/components/api.html#configuration-variables
encryption_key: "9zgsw5h/VOhDmsTWB1QvEQgMY3/GxGDSnQrSxv6fs90="
# https://esphome.io/components/ota.html
ota_password: albionboxes
# for albionboxes/prod_volcano_goober.yaml
volcano_mac_address: "C9:C9:C4:C4:D3:8F"
# for albionboxes/prod_gaggia_timer.yaml
gaggia_timer_alarm_media_file_path: "http://10.0.1.121:8123/local/simple_alarm.mp3"
# for all the rufus ones
rufus_url: "http://10.0.1.69:5000"
```

## Resources

* https://esphome.io/guides/faq.html?highlight=secrets#tips-for-using-esphome
* https://www.home-assistant.io/docs/configuration/splitting_configuration/
