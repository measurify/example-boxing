# Design and development of an embedded system for physical activity

This paper has been written with the aim of measuring and recognizing the blows performed by an athlete in the field of martial arts, more precisely in boxing. In this specific case, the recognition of three types of shots (cross, left hook and right hook) is required. Through the sensors applied on the Arduino Nano 33 BLE Sense Rev2 board accelerometer and gyroscope values were measured during movements; then the data was transmitted via the BLE (Bluetooth Low Energy) connection on the board to a Flutter application installed on a mobile device and then sent to a Cloud API (application programming interface) called Measurify. Once the collection of the dataset was finished, a machine learning algorithm was used to generate a neural network model capable of classifying in real time which of the three chosen actions was carried out by the athlete.

## Quick start
To setup the embedded system, the following steps need to be followed:

* Install Arduino IDE.

* Inside the IDE settings, add your board.

* Install the following libraries: Arduino_APDS9960, Arduino_LPS22HB, Arduino_HS300x, Arduino_BMI270_BMM150


To setup the mobile device, the following steps need to be followed:

* Install Visual Studio Code.
* Install the Flutter plugin (Flutter SDK 3.10.6)
* Open the activity_tracker (inside the folder client in this repository).
* Now the client application is ready to be debugged on a device.