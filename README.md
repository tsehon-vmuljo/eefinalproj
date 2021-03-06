# EE250 Final Project - MindUno: An IoT System to Collect and Visualize Brianwave Data
### Team Members: 
Tyler Sehon, Victor Muljo
### **Demo Link:** https://drive.google.com/file/d/1gvVWAInyaOYTnaAPWKdwba9XMVyLUbCn/view?usp=sharing

## **Instructions to run code:**

1. On ArduinoUNO
   - Upload arduino_tx.ino to the ArduinoUno via the ArduinoIDE (must remove Rx for the code to allow the code to upload). 
2. On RaspberryPi, run the rpi_publish.py program:
   - ```python3 rpi_publish.py```
3. On virtual machine:
   - ```sudo systemctl start influxdb```
   - ```sudo systemctl start grafana-server```
   - run mqtt_influx_bridge.py
     - ```python3 mqtt_influx_bridge.py```

## Libraries used:
- [Paho MQTT Client](https://github.com/eclipse/paho.mqtt.python)
- [Serial](https://pythonhosted.org/pyserial/index.html)
- [time](https://docs.python.org/3/library/time.html)
- [datetime](https://docs.python.org/3/library/datetime.html#module-datetime)
- [InfluxDB Client](https://github.com/influxdata/influxdb-python)
- [Arduino Brain Library](https://github.com/kitschpatrol/Brain.git)
