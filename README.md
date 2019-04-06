# LG-Webos-Remote
Picture Elements lovelace card for LG WebOS tvs

Similar to the Roku Remote I've shared, I wanted to have a clickable remote control within Home assistant for my new LG WebOStv so I took advantage of a few things to stitch one together.

I am controlling the power toggle on the TV using the built in Media player services in home assistant + the Wake on Lan feature in the docs.

For most all other commands (up, down, click,etc), I used lgtv2mqtt thanks to hobbyquaker - https://github.com/hobbyquaker/lgtv2mqtt

I took the remote image from here,https://dribbble.com/shots/5363712-Universal-TV-Remote-App-Design
And used the picture elements lovelace card to display it and stack buttons over top.

Prerequisites: 

- installed LGWebOS component and WOL for powering on: https://www.home-assistant.io/components/webostv/
- installed and functional lgtv2mqtt: https://github.com/hobbyquaker/lgtv2mqtt
- Home Assistant with Lovelace + MQTT
- Other things I cant think of ???

Steps to setup:

1) Copy the remote.png image into your /config/www/ folder

2) Copy the lovelace_remote.yaml contents into a manual card or into your lovelace.yaml directly

3) Replace the Media player entity ids with your entity id

4) Replace the MQTT topic with whatever you called it. In the file, I use LG/#, but the default for lgtv2mqtt is lgtv/#


*Notes

Red - Netflix
Green - Hulu
Yellow - Plex
Blue - Amazon Prime
Smart - Web Browser (set homepage in browser to info page of home assistant for weather and things)
input - Doesnt do anything
Info - Set to CC, but doesn't seem to be doing anything in Netflix (too lazy to test more)
Hamburger icon - Not set to anything
