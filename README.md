# modbus

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
+1,3,m,1,9600,GRW,1,10,0104040026,0104040028,0104040005,0104040009
1,010400ffffffff@i0:10,Einspeisestrom,A,mainsc,1
1,010400ffffffff@i1:10,Einspeiseleistung,W,mainsw,1
1,010400ffffffff@i2:10,string 1 unten,W,s1w,1
1,010400ffffffff@i3:10,string 2 oben,W,s2w,1
```

### Variante (0BBD => Register 3005)
```
>D

>B
=>sensor53 r

>M 1
+1,16,m,1,9600,GRW,17,10,01040BBD
1,010404UUuuUUuu@i0:10,Einspeisestrom,A,mainsc,1
```
