# Offline Homeassistant-solar-battery-charge-prediction
Homeassistant solar battery charge prediction with display card.
Works plug and play with the modbus sungrow integration for HA (https://github.com/mkaiser/Sungrow-SHx-Inverter-Modbus-Home-Assistant)

<img width="605" alt="Bildschirmfoto 2023-05-07 um 09 57 38" src="https://user-images.githubusercontent.com/122117318/236665268-436fb44c-4a21-4e54-83fc-a4d706aa5e6d.png">
(first row is only shown when there is no production/ second and third row is shown when there is production.

# Features
all features are tested and only approximate real circumstances!

* fully offline!
* predict battery state at evening after charging
* predict battery state at morning after decharging
* predict battery charging time
* predict minimum charge needed to get over night
* predict time left of solar
* predict start of charging
* example lovelace card (mushroom required)

# ToDo
any contributions to improve the code are appreciated!
* compleate english translation (most entitys have english description in code)
* improve konfiguration
* improve accuracy
* sometimes the prediction fails by calculating negative percentages because of insufficient solar. this should be limited to realistic values (0-100%)
* use local weather data to improve prediction

# Installation
please contribute ANY upgrades to the card or algorythm thia helps everybody!
1. copy all files oft the battery-predict.yaml into your custom yaml integrations folder
2. make changes for your individual setup (set entity ids battery size, avg consumtion...)
3. copy the card as a manual yaml config into lovelace. !mushroom required!
4. edit the current production of solar entity in the conditional cards 


_

THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
