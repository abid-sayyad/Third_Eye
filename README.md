# Third Eye
# Workplace Safety

Safety is important, especially when you work in the industrial sector. For example, mining can cause respiratory illnesses, high blood pressure, poisoning and various other disorders that can last a lifetime, if not outright killing you.

This creates a need to be able to monitor employee health/vitals and environmental conditions. Being able to will mean that you can:
- Respond quickly to emergencies
- Track potential risks
- Monitor worker safety and physical health.

# Our Project

With this in mind, our group decided to create a device that uses sensors to track and transmit data to a website and via SMS in real-time.

![image](https://user-images.githubusercontent.com/62711442/156880427-f405e99a-ceaf-44ef-a740-b3499f905b86.png)

- Four sensors monitor heart rate, air quality, temperature and current location.
- The device uses the SIM900 GSM Module to send SMS alerts in case of any of the readings indicate a potential crisis (by passing a threshhold value).
- It also sends a request to the website with the sensor data.
- The website then stores the data, and you can look at the new values once refreshed as its updated.

![gif (2)](https://user-images.githubusercontent.com/62711442/156880545-ae12d377-9c7c-4833-b649-35f74c2bc38b.gif)

# Setting the Project Up

On the hardware side, we've used: 
- Raspberry Pi Pico
- MQ135
- MQ9
- Pulse Sensor
- IR Body temp sensor
- SIM900 GSM Module

As for the website, you can configure your device to send updates to the website in this form:

``` https://ntl-2022.herokuapp.com/update/APIKEY=694201a/PULSE=<value>/TEMP=<value>/MQ135=<value>/MQ9=<value>/LOC=<value> ```
- `LOC` should be in the form of `<lat>,<long>` 

Otherwise, you can also just edit the values and do it from your browser just to see how it looks like.

The website has been done with Flask and vanilla HTML/CSS/JS.

# To Do

- Respond to update requests via SMS
- Updating the website's values better (Right now, it just refreshes the page every few seconds)
- Adding the ability to view several users' data under one account/multiple accounts

# Screenshot of Website

![image](https://user-images.githubusercontent.com/62711442/156881019-6dad64b6-2e71-47b4-8b61-a73e71682b31.png)

# [Link to Site](https://ntl-2022.herokuapp.com/)

# Contributors

| <p align="center">![Lasya](https://github.com/lasyapan.png?size=128)<br>[Lasya](https://github.com/lasyapan)</p> | <p align="center">![Aniruddha Chatterjee](https://github.com/ronsys11.png?size=128)<br>[Ronak](https://github.com/ronsys11)</p> | <p align="center">![Abid](https://github.com/abid-sayyad.png?size=128)<br>[Abid](https://github.com/abid-sayyad)</p> |
| ---------------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------- |
