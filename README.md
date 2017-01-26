# smart-home-monitoring
Monitor your Smart Home, Home Server, Home Network devices and so on with influxdb, telegraf, mqtt and grafana and others

I have got a very basic smart home setup at home. FritzBox as VDSL2 modem, a HP MicroServer as Home Server, an Ubiquiti Edgerouter X-SFP as distribution an PoE Switch for various WiFi Hardware (Ubiquiti Unifi AC-Lite for home network) and maybe a Ubiquiti Unifi AP for Freifunk Hochstift in a later stage.

Now i want to add some temperatur sensors with ESP8266 and DHT22 from WeMos in the future, so i would need to have a logging chain and data visualisation backend for humidity and temperatur.

So for starters i am starting this config drop / howto space on github, so maybe someone finds it usefull or wants to add some improvemnets (MR/PR are verrrrry welcome)

This is how it looks like as of now (Jan 2017):

Ubiquiti Edgerouter X-SFP Data collected via Telegraf via SNMP)
![alt tag]https://github.com/northalpha/smart-home-monitoring/blob/master/img/EdgeRouterDashboard.png

Home Server
![alt tag]https://github.com/northalpha/smart-home-monitoring/blob/master/img/TelegrafDashboard.png

Please see the Wiki here for more step by step HowTos, which is basically meant to be a runbook for me if i have to set it up again :)

Idea and based on (mainly:) https://lkhill.com/using-influxdb-grafana-to-display-network-statistics/ and https://www.dev-eth0.de/blog/2016/12/06/grafana_snmp.html
