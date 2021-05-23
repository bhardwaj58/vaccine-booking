<h1 align="center">COVID-19 Vaccination Slot Booking Script</h1>

<div align="center">



</div>




## Setup Guide for iOS

### Using Shortcuts app
1. Open the shortcuts app
2. Tap on the + button at the top right
3. Tap on `Create Personal Automation`
3. Select the `Message` option
4. Put `CoWIN` in the Message Contains option & leave everything blank. Tap on Next button
5. Tap on `Add action` and search for the option `Set Variable`. Give the variable name `text` and input as `Shortcut Input`
6.     Then add another action and select `URL` and paste the url: https://kvdb.io/ASth4wnvVDPkg2bdjsiqMN/99XXXXXXXX replace 99XXXXXXXX with your phone number
7. Then add another action and select `Get Contents of Url`. Click on show more. Change the method to `PUT`. Request Body to `File` and in the file row tap on `Choose Variable` and select `text` which we defined in Step 6.
8. Click Next and save this automation.
9. Clone this repository
Go to `src` directory and run the script  `cd src && python covid-vaccine-slot-booking.py`
15. On Mac I had to do the following too
     - `brew install python-tk`
     - `brew install SoX`
18. Run the script, enter your phone number. 
19. Now as soon as OTP is recieved you will also get a notification from shortcuts app. Long press it and click on run. It will start OTP auto read process.
20. Use the steps given below to enter your preferences. 
21. Now whenever the script session expires, it will send the notification  described in step 13 and repeat the process to trigger OTP auto read. 
22. It is recommended that you set a different notification tone for this notification to be able to distinguish.
23. Hopefully you get the slot
24. Stay healthy and stay safe!




**Tips:** 

run : python -m pip install -r requirements.txt`
run : python src\covid-vaccine-slot-booking.py

