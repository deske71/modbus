# modbus

Growatt Register PDF
https://community.symcon.de/uploads/short-url/jFo2xrUpTus03y9fWeYrp0Dbfng.pdf

ModbusSerialConfig 3

ModbusBaudrate 115200

ModBusSend {"DeviceAddress": 1, "FunctionCode": 3, "StartAddress": 0, "Type":"int16", "Count":12}

ModBusSend {"DeviceAddress": 1, "FunctionCode": 6, "StartAddress": 10, "Type":"int16", "Count":1, "Values":[44]}


https://github.com/ClassicDIY/ModbusTool

https://github.com/arendst/Tasmota/discussions/14810

https://ottelo.jimdofree.com/stromz%C3%A4hler-auslesen-tasmota/

## Serial Communication

ModBusSlave starten

https://github.com/gthvidsten/open-serial-port-monitor/releases/tag/v1.0.5988.23754

Main Menu -> Configure Module -> TX und RX auf "Serial TX" und "Serial RX" setzen

SerialConfig 3

SerialSend "meinString"

## Tasmota SML

https://github.com/ottelo9/tasmota-sml-images
```
>D

>B
=>sensor53 r

>M 1
+1,16,m,1,9600,GRW,17,10,01040BBB,01040BCF,01040BD1,01040BEF,01040BEB
1,010404UUuu@i0:10,PV Spannung,V,pvspannung,1
1,010404UUuuUUuu@i1:10,Leistung,W,output,2
1,010404UUuu@i2:100,Netzfrequenz,Hz,ntzfrqnz,3
1,010404UUuuUUuu@i3:10,Heute,k,today,3
1,010404UUuuUUuu@i4:10,Gesamt,kWh,total,2
```
