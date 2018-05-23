# Onling Parking System: Android Application

Android Application screenshots:

Login          |  Parking Zone
:-------------------------:|:-------------------------:
![Login](https://i.imgur.com/L3NcuuP.png)  |  ![Parking Zone](https://i.imgur.com/xw94ioh.png)

Log-In: Users able to create an account from the login page of the application. In the case of when user forgets their password, they will also have the option of resetting it by clicking on the "Reset Password" button. After entering the email address in the reset password field, an email is sent to the user with instructions to reset the password. When the user successfully verifies their email address with the confirmation link sent to their email upon account creating, they are able to login into the application. A token is generated and stored in the device to validate the users current session and to make API requests to the server.

Parking Slot          |  Billing
:-------------------------:|:-------------------------: 
![Parking Slot](https://i.imgur.com/KtPEXK8.png)  |  ![Billing](https://i.imgur.com/Kk045Dm.png) 

List of Parking Zones and Slots: When user successfully logs on, the user is presented with a list of parking structures/zones available for selection. When more zones are available, they can be added into our database then the application will be able to reflect the current changes. By selecting a zone from the list prior, users will be able to then select a parking space that are given a unique id. The selected option will be the parking space the user wants to park their car. When user selects an unoccupied parking space, they are presented with a form where they can select the number of hours to park their car. After submitting the request, the microcontroller will detect whether the car is currently occupied on the spot and proceed to the close the gate, otherwise waits until the car parks to close.


Billing Information: In order to make a purchase for a parking space, users are first required to enter their billing information which supports debit and credit cards. After entering a valid billing information, user is also given the option to remove their billing information.

Purchase History          |  End Session
:-------------------------:|:-------------------------: 
![Purchasing History](https://i.imgur.com/d18qqGU.png)  |  ![End Session](https://i.imgur.com/UfpxrnL.png) 

Purchase History: Users are able to view past purchases by selecting the "Purchase History" option in the navigation drawer. On this section, users are able to see completed and in progress purchases. If the parking space is currently in progress, user is given the option to terminate the session early. Upon clicking the end session, the server will notify the microcontroller to open the gate. 


## What is this?

The Online Parking service provides and integrated experience in payment parking systems. The Particle micro controller enables parking space tracking using an ultrasonic sensor. It also controls the position of the gate, whether it's closed or open. The Android companion app provides a GUI interface for customers to conveniently monitor and pay for their parking. The Node.js server links the Android application and particle micro controller by performing the database connection and providing the logic required to manage a parking system. The server is hosted on Google Cloud using an app engine and deployed using Google Cloud Services.

## Dependencies

The focus of this project lies on the view layer and app navigation. It uses the following dependencies:

- AppCompat Support Library
- Support Design Library
- Support Card View Library
- Butterknife
- Glide 
- Android Asynchronous Http Client

## Supported devices

The application supports every device with a SDK level of at least 14 (Android 4+).

### About

Android Application base developed using Andreas Schrade Material Design Android Template. Android and Java backend was developed by Alex Tran and Kevin Ngo.



 

