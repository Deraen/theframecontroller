# The Frame Art mode controller

Control Samsung The Frame Art Mode using ESPHome to talk to the One Connect box
with RS232/Ex-link. You need ESP8266 or ESP32 and a UART/TTL to RS232
converter, like something using MAX2323 chip.

No custom uart component, reading the status is done using 
esphome uart bus debugging, with additional code parsing the received
bytes after 100ms of silence.

## Compile

`esphome compile samsung.yaml`

## Upload

`esphome upload samsung.yaml --device 192.168.42.48`

## Notes

- https://www.remotecentral.com/cgi-bin/forums/viewpost.cgi?1412783
- https://www.reddit.com/r/TheFrame/comments/x3hhcf/comment/imqz1p8/?utm_source=reddit&utm_medium=web2x&context=3
- https://docs.google.com/spreadsheets/d/18s25cj1RK-9qR7_ydXHL_P58DpiaWWgu/edit#gid=953994101
- https://www.seeedstudio.com/RS-232-To-TTL-Conveter-MAX3232IDR-p-2851.html
- https://support.justaddpower.com/kb/article/16-samsung-rs232-control-exlink/
- https://github.com/phillipsnick/samsung-tv/blob/master/lib/app.js
- https://community.home-assistant.io/t/how-to-uart-read-without-custom-component/491950
