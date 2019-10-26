# Server Client
To run the program use the following ampy command

## Note 
- We will use ```ampy``` to put the code in the ESP8266 picocom to run the program inside the ```terminal```
- Use two different system for each ESP8266
- Connect the system which you want to make server with the WiFi before starting the server
- This communication will be half duplex and the system will wait until the information is not received or sent

## MAC OS
```bash
    ampy --port /dev/tty.SLAB_USBtoUART put server_client.py main.py
```

```bash
    picocom /dev/tty.SLAB_USBtoUART -b 115200
    
    Press ctrl + C to end the process
    import main
```

## Linux
```bash
    ampy --port /dev/ttyUSB0 run accesspoint.py
```

```bash
    picocom /dev/ttyUSB0 -b 115200
    
    Press ctrl + C to end the process
    import main
```
