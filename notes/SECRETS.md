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
```

## Resources

* https://esphome.io/guides/faq.html?highlight=secrets#tips-for-using-esphome
* https://www.home-assistant.io/docs/configuration/splitting_configuration/
