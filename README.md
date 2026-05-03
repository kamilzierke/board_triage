# Board Triage ESPHome Packages

Public ESPHome package files used by the local board triage workflow.

The triage script flashes a first validated ESPHome build, then rebuilds the device YAML with a per-board `dashboard_import` URL pointing at one of these files. That lets ESPHome Dashboard/Builder adopt the board with the right project metadata instead of relying only on Home Assistant device discovery.

## Packages

- `boards/lolin_c3_pico.yaml` - LOLIN/WEMOS C3 Pico v1.0.0, ESP32-C3FH4, WS2812 RGB LED on GPIO7 with `rgb_order: RGB`, BOOT button on GPIO9, optional battery ADC on GPIO3 after `BAT_AD` solder jumper.

## URL format

```text
github://kamilzierke/board_triage/boards/<profile_id>.yaml@main
```
