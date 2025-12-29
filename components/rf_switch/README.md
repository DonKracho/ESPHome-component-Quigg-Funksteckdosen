```yaml
# example configuration:

# device specific components
external_components:
  #source: github:DonKracho/ESPHome-component-Quigg-Funksteckdosen/components@main
  refresh: 0s

switch:
  - platform: rf_switch
    name: 'rf switch'
    output: rf_transmitter
    channel: 0 # 0:default   1:different rolling code sequence

output:
  - platform: rf_outlet
    id: rf_transmitter
    pin: GPIO6
    repeat: 6 # optional, default: 6
```
