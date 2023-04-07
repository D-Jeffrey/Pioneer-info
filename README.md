
## BLUF
You should go to https://github.com/crowbarz/ha-pioneer_async and use that version if you are looking for something reliable to control your Pioneer.



# Developer Notes and learnings


in some models the port number is adjusted in the network setup.

http://192.168.4.44/1000/network_stanby.asp
(Does not work on my VSX-925, but should work for others?)


And the radio stations is this link for me.
```
 http://192.168.4.44/InternetRadioSettingListHandler.asp
{
	"R":[
	{
		"C":1,
		"T":"CBC Radio One",
		"U":"http://origin.www.cbc.ca/mrl2/livemedia/cbcr1-calgary.asx"
	},
	{
		"C":2,
		"T":"CFFR - 660 News",
		"U":"http://38.99.208.186/660NEWS"
	},
	{
		"C":24,
		"T":"FM Nirai",
		"U":"http://www.simulradio.jp/asx/fm-nirai.asx"
	}
	]
}	
```

The StatusHandlder.asp give Zone and channel names.  Actually, it looks like a one stop current values page.  File this other interesting to know, but we have all that.


```
http://[192.168.4.44/StatusHandler.asp](http://192.168.4.44/StatusHandler.asp)

{
	"S":1,
	"B":0,
	"Z":[
		{"P":1,"V":93,"M":0,"I":[4,25,5,15,10,14,19,20,21,17,1,3,2,27,26,33],"C":5},
		{"P":0,"V":-1,"M":0,"I":[4,5,15,10,14,1,3,2,33],"C":4}
	],
	"L":1,
	"A":5,
	"IL":[
		"Wii           ",
		"Bluray        ",
		"TV/SAT",
		"DVR/BDR",
		"VIDEO 1",
		"VIDEO 2",
		"CabIe         ",
		"Computer      ",
		"Amazon FireTV ",
		"iPod/USB",
		"CD",
		"CD-R/TAPE",
		"TUNER",
		"SIRIUS",
		"INTERNET RADIO",
		"ADAPTER PORT"
	],
	"H":0
}
```



### For VSX-31, VSX-30	uses Port 23

#### About Network Standby
This setting allows the IP Control function for operating the receiver from a IP control system connected on the same LAN as the receiver to be used even when the receiver is in the standby mode.
1. Select �Network Standby� from the Network Setup menu.
2. Then set to "ON"

Some models include this Network Standy which allows the power on commands to work.  You can access this using the System Setup menu, Network setup, Network Standby.

VSX-924 - Yes
VSX=925 - No

# ?RGD Command
Does not work on older models Pre-2016

# FL does not work on older models


## Pioneer Models that have a LAN (and/or WiFi)  
(Source hifiengine.com) - 56 devices

See [Pioneer Models in JSON](pioneermodel.json)
Model	|	Year	|	Digital Ports
----	|	----	|	----
SC-05	|	2008	|	coaxial, optical, USB, LAN
SC-07	|	2008	|	coaxial, optical, USB, LAN
SC-1223	|	2013	|	coaxial, optical, USB, LAN
SC-1224	|	2014	|	coaxial, optical, USB, LAN
SC-1228	|	2013	|	coaxial, optical, USB, LAN
SC-2022	|	2012	|	coaxial, optical, USB, LAN, WiFi, BT
SC-2024	|	2014	|	coaxial, optical, USB, LAN
SC-25	|	2009	|	coaxial, optical, USB, LAN
SC-71	|	2013	|	coaxial, optical, USB, LAN
SC-81	|	2014	|	coaxial, optical, USB, LAN
SC-82	|	2014	|	coaxial, optical, USB, LAN
SC-85	|	2014	|	coaxial, optical, USB, LAN
SC-87	|	2014	|	coaxial, optical, USB, LAN
SC-LX502	|	2017	|	coaxial, optical, USB, LAN, Wifi, BT
SC-LX58	|	2014	|	coaxial, optical, USB, LAN
SC-LX71	|	2008	|	coaxial, optical, USB, LAN
SC-LX72	|	2009	|	coaxial, optical, USB, LAN
SC-LX73	|	2010	|	coaxial, optical, USB, LAN
SC-LX75	|	2011	|	coaxial, optical, USB, LAN
SC-LX78	|	2014	|	coaxial, optical, USB, LAN
SC-LX801	|	2016	|	coaxial, optical, USB, LAN, WiFi, BT
SC-LX81	|	2008	|	coaxial, optical, USB, LAN
SC-LX82	|	2009	|	coaxial, optical, USB, LAN
SC-LX83	|	2010	|	coaxial, optical, USB, LAN, BT
SC-LX85	|	2011	|	coaxial, optical, USB, LAN
SC-LX88	|	2014	|	coaxial, optical, USB, LAN
SC-LX901	|	2016	|	coaxial, optical, USB, LAN, WiFi, BT
VSX-1120	|	2010	|	coaxial, optical, USB, LAN, BT
VSX-1121	|	2011	|	coaxial, optical, USB, LAN, WiFi, BT
VSX-1124	|	2014	|	coaxial, optical, USB, LAN
VSX-1129	|	2014	|	coaxial, optical, USB, LAN
VSX-2020	|	2010	|	coaxial, optical, USB, LAN
VSX-2021	|	2011	|	coaxial, optical, USB, LAN, WLAN, BT
VSX-30	|	2010	|	coaxial, optical, USB, LAN, BT
VSX-32	|	2010	|	coaxial, optical, USB, LAN
VSX-33	|	2010	|	coaxial, optical, USB, LAN
VSX-43	|	2013	|	coaxial, optical, USB, LAN, BT
VSX-44	|	2014	|	coaxial, optical, USB, LAN, WiFi, BT
VSX-51-2	|	2011	|	coaxial, optical, USB, LAN, WLAN, BT
VSX-52-2	|	2011	|	coaxial, optical, USB, LAN, WLAN, BT
VSX-527	|	2012	|	coaxial, optical, USB, LAN, BT
VSX-529	|	2014	|	coaxial, optical, USB, LAN
VSX-53-2	|	2011	|	coaxial, optical, USB, LAN, WLAN, BT
VSX-60	|	2012	|	coaxial, optical, USB, LAN, WLAN, BT
VSX-80	|	2014	|	coaxial, optical, USB, LAN
VSX-823	|	2013	|	coaxial, optical, USB, LAN, BT
VSX-8231	|	2013	|	coaxial, optical, USB, LAN, BT
VSX-824	|	2014	|	coaxial, optical, USB, LAN
VSX-827	|	2012	|	coaxial, optical, USB, LAN, BT
VSX-830	|	2015	|	coaxial, optical, USB, LAN, WiFi, BT
VSX-832	|	2017	|	coaxial, optical, USB, LAN, BT
VSX-924	|	2014	|	coaxial, optical, USB, LAN
VSX-925	|	2010	|	coaxial, optical, USB, LAN
VSX-932	|	2017	|	coaxial, optical, USB, LAN, Wifi, BT
VSX-933	|	2018	|	coaxial, optical, USB, LAN, Wifi, BT

## Pioneer Models that do NOT have a network connection

Model	|	Year	|	Digital Ports
----	|	----	|	----
SC-1222	|	2012	|	coaxial, optical, USB
SC-1227	|	2012	|	coaxial, optical, USB
SC-1323	|	2013	|	coaxial, optical
SC-1328	|	2013	|	coaxial, optical
SC-1522	|	2012	|	coaxial, optical, USB
SC-1523	|	2013	|	coaxial, optical
SC-1525	|	2010	|	coaxial, optical, USB
SC-1526	|	2011	|	coaxial, optical, USB
SC-1527	|	2012	|	coaxial, optical, USB
SC-35	|	2010	|	coaxial, optical, USB
SC-55	|	2011	|	coaxial, optical, USB
SC-61	|	2012	|	coaxial, optical, USB
SC-63	|	2012	|	coaxial, optical, USB
SC-65	|	2012	|	coaxial, optical, USB
SC-67	|	2012	|	coaxial, optical, USB
SC-72	|	2013	|	coaxial, optical
SC-75	|	2013	|	coaxial, optical
SC-77	|	2013	|	coaxial, optical, USB
SC-LX56	|	2012	|	coaxial, optical
SC-LX57	|	2013	|	coaxial, optical
SC-LX76	|	2012	|	coaxial, optical, USB
SC-LX77	|	2013	|	coaxial, optical, USB
SC-LX86	|	2012	|	coaxial, optical, USB
SC-LX87	|	2013	|	coaxial, optical, USB
VSX-1122	|	2012	|	coaxial, optical, USB
VSX-1123 (1123-K)	|	2013	|	coaxial, optical
VSX-1128 (1128-K)	|	2013	|	coaxial, optical
VSX-2014i	|	2004	|	coaxial, optical
VSX-2016AV	|	2006	|	coaxial, optical
VSX-21	|	1999	|	coaxial, optical
VSX-21TXH	|	2009	|	coaxial, optical, USB
VSX-23TXH	|	2009	|	coaxial, optical, USB
VSX-321	|	2011	|	coaxial, optical
VSX-322	|	2012	|	coaxial, optical
VSX-323	|	2013	|	coaxial, optical, USB
VSX-324-K	|	2013	|	coaxial, optical
VSX-330	|	2015	|	coaxial, optical, USB
VSX-40	|	2011	|	coaxial, optical, USB
VSX-41	|	2002	|	coaxial, optical
VSX-415	|	2004	|	coaxial, optical
VSX-416	|	2006	|	coaxial, optical
VSX-417	|	2007	|	coaxial, optical
VSX-42	|	2012	|	coaxial, optical
VSX-420	|	2010	|	coaxial, optical
VSX-420-K	|	2010	|	coaxial, optical
VSX-422	|	2012	|	coaxial, optical
VSX-423	|	2013	|	coaxial, optical, USB
VSX-430	|	2015	|	coaxial, optical, USB, BT
VSX-515	|	2004	|	coaxial, optical
VSX-516	|	2005	|	coaxial, optical
VSX-517	|	2007	|	coaxial, optical
VSX-518	|	2007	|	coaxial, optical
VSX-520	|	2010	|	coaxial, optical
VSX-521	|	2011	|	coaxial, optical
VSX-522	|	2012	|	coaxial, optical
VSX-523	|	2013	|	coaxial, optical, USB
VSX-5231	|	2013	|	coaxial, optical, USB
VSX-523-K	|	2013	|	coaxial, optical, USB
VSX-524	|	2014	|	coaxial, optical, USB
VSX-5241	|	2014	|	coaxial, optical, USB
VSX-530	|	2015	|	coaxial, optical, USB, BT
VSX-531	|	2016	|	coaxial, optical, USB, BT
VSX-531D	|	2017	|	coaxial, optical, USB, BT
VSX-609RDS	|	2000	|	coaxial, optical
VSX-70	|	2013	|	coaxial, optical
VSX-709RDS	|	2000	|	coaxial, optical
VSX-815	|	2004	|	coaxial, optical
VSX-816	|	2005	|	coaxial, optical
VSX-817	|	2006	|	coaxial, optical
VSX-818V	|	2008	|	coaxial, optical
VSX-819H	|	2009	|	coaxial, optical
VSX-820	|	2009	|	coaxial, optical
VSX-821	|	2011	|	coaxial, optical
VSX-822	|	2012	|	coaxial, optical
VSX-826	|	2011	|	coaxial, optical, USB
VSX-9110 (TXV)	|	2006	|	coaxial, optical
VSX-915	|	2004	|	coaxial, optical
VSX-916	|	2005	|	coaxial, optical
VSX-917V	|	2007	|	coaxial, optical
VSX-918V	|	2008	|	coaxial, optical
VSX-919AH (K)	|	2009	|	coaxial, optical
VSX-920	|	2010	|	coaxial, optical
VSX-921	|	2011	|	coaxial, optical
VSX-922	|	2012	|	coaxial, optical, USB
VSX-923	|	2013	|	coaxial, optical, USB
VSX-9300TX	|	2004	|	coaxial, optical



Move to https://github.com/crowbarz/ha-pioneer_async


#### Work in Progress

| Model  | Port | Year | Network Standby | ZONES | FL | ?RGD | VOL |?PR|?FR| ?SVB | ?SSI | LAN/WiFi| USB |
| -----  |-----:|------|-----------------|-------|----| -----|-----|---|---|------|------|----|-----|
|VSA-1124|8102 |2014  | ?               | ?     | ?  | ?    | ?   |?  | ? | ?    | ?    | N   | N |
|VSA-1130|8102 |2015  | ?               | ?     | ?  | ?    | ?   |?  | ? | ?    | ?    | Y   | N |
|VSA-830 |8102 |2015  | ?               | ?     | ?  | ?    | ?   |?  | ? | ?    | ?    | N   | N |
|VSX-1120|8102 |2010  | ?               | ?     | ?  | ?    | ?   |?  | ? | ?    | ?    | N   | Y |
|VSX-1121|8102 |2011  | ?               | ?     | ?  | ?    | ?   |?  | ? | ?    | ?    | Y/Y | Y |
|VSX-1021|8102 |2011  | Y               | ?     | ?  | ?    | ?   |?  | ? | ?    | ?    | Y/Y | Y |
|VSX-925 |8102 |2010  | N               | 2     | N  | N    | Y   |Y  | Y | N    | N    | Y/N | Y |
|VSX-1025 |8102|2010  | N               | 2     | N  | N    | Y   |Y  | Y | N    | N    | Y/N | Y |
|VSX-924 |8102 |2014  | Y              | 2      | ?  | Y    | Y   |Y  | Y | ?    | ?    | Y/N | Y |
|VSX-922 |8102 |2012  | Y              | ?      | ?  | ?    | ?   |?  | ? | ?    | ?    | Y/Y | Y |
|VSX-1122|8102 |2012  | Y              | ?      | ?  | ?    | ?   |?  | ? | ?    | ?    | Y/Y | Y |
|VSX-529 |8102 |2014  | ?              | ?      | ?  | ?    | ?   |?  | ? | ?    | ?    | Y/N | Y |


### Reference
https://github.com/rwifall/pioneer-receiver-notes/blob/ec16e194f64860df4dcc2d105a57604a21a9c75c/README.md



|  SC | SC  |SC   | SC-LX  | VSX | VSX | VSX | VSX |
|--- |--- |--- |---    |--- |--- | ---| ---
|	SC-71	|	SC-1223	|	SC-2023	|	SC-LX57	|	VSX-45	| VSX-529		|	VSX-1025*| VSX-2021
|	SC-75	|	SC-1228	|		|	SC-LX77	|		|	VSX-830	|	VSX-1028|
|	SC-77	|	SC-1323	|		|	SC-LX78	|		|	VSX-923		|	VSX-1120|
|		|	SC-1328	|		| SC-LX87 		|		|	VSX-925*	|	VSX-1123|
|		|	SC-1523	|		|		|		|	VSX-930	|	VSX-1128|
|		|	SC-1528	|		|		|		|		|           |

 \* does not support sleep mode

```