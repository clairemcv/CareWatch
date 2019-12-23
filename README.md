# CareWatch

Monitored living project prototype suitable for an elderly person.
To check they are well and maintaining their daily routine, i.e. moving about and making cups of tea.

The senseHat sensor records changes of temperature and accelerator data to imitate this action.

Rpi collects temperature and (accelerator) movement data and sends it to Wia and Thingspeak

Wia displays temperature and accelerator movement data in widgets. I also subscribed to Wia MQTT events and logging in from another location all events are recorded. 

Wia widgets are embedded in a live webpage 
http://carewatch.surge.sh  

Thingspeak 

https://thingspeak.com/channels/942131
https://thingspeak.com/channels/921244

Thingspeak displays temperature and accelerator movement data in channels.

Tweet React so if temperature rises above 38 i.e. kettle on, tweet sent out
https://twitter.com/Claire28104113

IFTT applet established so upon activated tweet, an email is sent.

Blynk App

Rpi collects temperature and (accelerator) movement data and sends to Blynk.

Blynk displays current temperature and Kettle Last Used Time in a ‘super chart’ that gives a live feed of current temperature and movement. It can also displays this data for up to a year in various increments.

Also sends Accelerator data to Thingspeak with a web hook.
