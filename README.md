# lib_webrtc_kea
This repo runs 'WebRTC' using the chrome driver on a Mission Computer called KEA based on Raspberry Pi.
***
### 1. Install
- `Chrome Driver` - WebDriver for running WebRTC
```shell
sh ready_to_WebRTC.sh
```
- `xvfb` - for virtual display
```shell
sudo apt-get install xvfb
```
- python library - including paho-mqtt, seleniu, PyVirtualDisplay and etc.
```shell
pip3 install -r requirements.txt
```


### 2. Run
- `lib_webrtc_kea.py` - The arguments are WebRTC_URL and Drone_Name.
```shell
python3 lib_webrtc_kea.py {{WebRTC_URL}} {{Drone_Name}}
```


### 3. Convert to App
- Install python library
```shell
pip3 install pyinstaller
```
- Convert
```shell
python3 -m PyInstaller -F lib_webrtc_kea.py 
```