# LG-Webos-Remote
Picture Elements lovelace card for LG WebOS tvs

Similar to the Roku Remote I've shared, I wanted to have a clickable remote control within Home assistant for my new LG WebOStv so I took advantage of a few things to stitch one together.

I am controlling the power toggle on the TV using the built in Media player services in home assistant + the Wake on Lan feature in the docs.

For most all other commands (up, down, click,etc), I used lgtv2mqtt thanks to hobbyquaker - https://github.com/hobbyquaker/lgtv2mqtt

I took the remote image from here,https://dribbble.com/shots/5363712-Universal-TV-Remote-App-Design

And used the picture elements lovelace card to display it and stack buttons over top.

You'll need to make sure you overwrite your Media player entities with your entity name, and your MQTT topic with whatever you called it.

