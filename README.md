## Social Distancing App

Social Distancing App that can assist limit interaction between people within a 2-meter range

BLE and proximity-based applications are useful for limiting contact between people while using RSSI to gauge their distance from one another.

Transferring data between devices via GATT Client and GATT Server, which enables the identification of user involvement.

The app transfers data between devices via GATT Client and GATT Server, enabling the identification of user involvement. The user interface provides a simple, easy-to-use dashboard to view the current distance between users and receive alerts when necessary.

## Prerequisites
* Android Studio installed on your system
* An Android device with developer options enabled
## Installation

Steps to run Social Distancing App on Android.


 1. clone the project using below command

    ```bash 
    git clone https://github.com/siddheshgarud/Social-Distancing-by-Siddheshgarud
    ```

 2.  Open Android Studio and select `Open an existing Android Studio project` from the Welcome screen or use `File > Open` from the main menu.

3. Navigate to the folder containing the project you want to open and select it.

4. Android Studio will import the project and build the project structure.

5. Connect your Android device to your computer or start an emulator.

6. In the toolbar, select the `device` or `emulator` you want to run the app on.

7.  Click the Run button in the toolbar or use the `Run > Run app` command from the main menu.

8.  Android Studio will build the app and install it on your device or emulator.

9.  Once the app is installed, it will launch automatically.


## Features

- Bluetooth-based proximity detection to identify other app users in the vicinity.
- Real-time monitoring of distance between users using Bluetooth signal strength.
- Customizable alert settings based on distance thresholds.
- History log to keep track of previously detected users with timestamps and distance measurements.

## Demo

will eventually upload more pictures

* Main page of the app

<img src="https://raw.githubusercontent.com/siddheshgarud/Social-Distancing-by-Siddheshgarud/master/Screenshots/Screenshot.jpeg"  width="300" height="500" />

* When you first launch the App, it may request permission to access your device's Bluetooth functionality.

<img src="https://raw.githubusercontent.com/siddheshgarud/Social-Distancing-by-Siddheshgarud/master/Screenshots/Screenshot5.jpeg"   width="300" height="500"/>

* Main page when no user is detected

<img src="https://raw.githubusercontent.com/siddheshgarud/Social-Distancing-by-Siddheshgarud/master/Screenshots/Screenshot12.jpeg"   width="300" height="500" />

* If a user is detected violating social distancing guidelines, the App will generate an 'Alert' to notify the user, and the importance of risk level will increase depending on the distance.

<img src="https://raw.githubusercontent.com/siddheshgarud/Social-Distancing-by-Siddheshgarud/master/Screenshots/Screenshot11.jpeg"   width="300" height="500" />

* The App maintains a history of previously detected users, including the accurate time of detection, the proximity distance of the user, and an assessment of the associated risk level. 

<img src="https://raw.githubusercontent.com/siddheshgarud/Social-Distancing-by-Siddheshgarud/master/Screenshots/Screenshot7.jpeg"   width="300" height="500" />

## Tech Stack

**Client:** Java

**HardWare:** BLE  , Proximity Sensor

**Software:** RSSI , GATT Server , GATT Client



## Working
The Social Distancing app utilizes the BLE advertising feature to broadcast its presence to nearby devices. It periodically sends out advertising packets containing information about the app, such as its unique identifier and proximity status. The advertising packets are received by other nearby devices that are scanning for BLE advertisements.

The proximity status of the nearby devices is determined by measuring the RSSI of the received advertising packets. RSSI is a measure of the signal strength of the received BLE signals, and it can be used to estimate the distance or proximity between devices. For example, a stronger RSSI value may indicate that the devices are closer to each other, while a weaker RSSI value may indicate that they are further apart.

The app uses GATT servers, which are part of the BLE protocol, to expose data about its proximity status to other devices in a standardized way. The app's GATT server stores information such as the device's unique identifier and proximity status.

When a nearby device receives an advertising packet from the app, it can read the data from the app's GATT server to obtain information about its proximity status. For example, the GATT server may store the RSSI value of the advertising packet, which can be used to estimate the distance between the devices.

Based on the proximity status of the nearby devices, the app can trigger alerts or notifications to remind users to maintain social distancing. For example, if the RSSI value indicates that two devices are within a certain threshold distance, the app may alert the users to maintain a safe distance from each other.

* Flowchart of the system

<img src="https://raw.githubusercontent.com/siddheshgarud/Social-Distancing-by-Siddheshgarud/master/Screenshots/Screenshot6.jpeg"  width="400" height="600" />


## Explanation



**BLE:** BLE stands for Bluetooth Low Energy, which is a wireless personal area network technology designed to provide low-power communication for short-range devices. It is often used in IoT devices, wearable technology, and healthcare applications. BLE is designed to consume less power than traditional Bluetooth technology and operates in the 2.4 GHz ISM band. 



**RSSI:** RSSI stands for Received Signal Strength Indicator and is a measure of the power present in a received radio signal. It is often used to determine the distance between a device and a nearby wireless transmitter, such as a Bluetooth or Wi-Fi device. The higher the RSSI value, the stronger the signal and the closer the device is to the transmitter. 


**GATT:** GATT (Generic Attribute Profile) is a key aspect of Bluetooth Low Energy (BLE) communication, which is used to define how two BLE devices transfer data.

**GATT Server:**  A GATT Server is a device that stores data and makes it accessible to other BLE devices. It contains a collection of data known as "services" and "characteristics". The services contain collections of data known as characteristics.

**GATT Client:** A GATT Client is a device that requests data from a GATT Server and can also write data to it. It communicates with the GATT Server by sending read and write requests to access and modify the data stored on the server.

In BLE communication, a GATT Client and a GATT Server can be either the same device or two separate devices. The GATT Client and Server exchange data using a well-defined protocol, which is used to create a communication link between the two devices.

* DFD Level 0

<img src="https://raw.githubusercontent.com/siddheshgarud/Social-Distancing-by-Siddheshgarud/master/Screenshots/Screenshot8.jpeg"  height="200"  />

* DFD Level 1

<img src="https://raw.githubusercontent.com/siddheshgarud/Social-Distancing-by-Siddheshgarud/master/Screenshots/Screenshot9.jpeg"  height="200" />

## Disclaimer

The Social Distancing App is not a substitute for professional medical advice or guidance. Users should continue to follow official health guidelines and regulations in their respective regions to ensure the safety and well-being of themselves and others.
## Authors

- [@Siddhesh Garud](https://in.linkedin.com/in/siddheshgarud)



