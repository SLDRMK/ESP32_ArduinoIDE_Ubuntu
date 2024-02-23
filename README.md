# Install Arduino IDE on Ubuntu for ESP32
### BY SLDRMK
1. Download AppImage from [Arduino Software](https://www.arduino.cc/en/software) and follow the steps from [Arduino Installation Tutorial](https://docs.arduino.cc/software/ide-v2/tutorials/getting-started/ide-v2-downloading-and-installing/) to set up the IDE.
2. Follow the instructions from [ESP32 Configration Instuctions](https://randomnerdtutorials.com/installing-the-esp32-board-in-arduino-ide-windows-instructions/).
3. Connect ESP32 board to USB pot and run the following scripts to check the USB port COM.
```
ls /dev/ttyUSB*
```
4. Run the following scripts to give arduino IDE accsess to the USB port.
```
$ sudo adduser <username> dialout
$ sudo chmod a+rw /dev/<ttyUSB*>
```
5. Test if the codes can be compiled and uploaded to the ESP32 board.

[CSDN](https://blog.csdn.net/szhmonkey/article/details/136075986)
