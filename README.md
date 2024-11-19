# modbus

ModbusSerialConfig 3

ModbusBaudrate 115200

ModBusSend {"DeviceAddress": 1, "FunctionCode": 3, "StartAddress": 0, "Type":"int16", "Count":12}

ModBusSend {"DeviceAddress": 1, "FunctionCode": 6, "StartAddress": 10, "Type":"int16", "Count":1, "Values":[44]}


https://github.com/ClassicDIY/ModbusTool

https://github.com/arendst/Tasmota/discussions/14810

## Serial Communication

https://github.com/gthvidsten/open-serial-port-monitor/releases/tag/v1.0.5988.23754

Main Menu -> Configure Module -> TX und RX auf "Serial TX" und "Serial RX" setzen

SerialConfig 3

SerialSend "meinString"
