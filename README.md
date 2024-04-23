# Offline Homeassistant-solar-forecast-and-battery-state-forecast
<a href="https://www.buymeacoffee.com/hauser1234" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Coffee" height="41" width="174"></a>

Homeassistant solar battery charge prediction with display card.
Works plug and play with the modbus sungrow integration for HA (https://github.com/mkaiser/Sungrow-SHx-Inverter-Modbus-Home-Assistant)

<img width="605" alt="Bildschirmfoto 2023-05-07 um 09 57 38" src="https://user-images.githubusercontent.com/122117318/236665268-436fb44c-4a21-4e54-83fc-a4d706aa5e6d.png">
(The first row is only shown when there is no production / second and third rows are shown when there is production.

If you like this repository please leave a star ⭐
# Features
All features are tested and only approximate real circumstances!

* fully offline!
* predict battery state in the evening after charging.
* predict battery state in the morning after discharging.
* predict battery charging time.
* predict the minimum charge needed to get overnight.
* predict the time left of solar.
* predict the start of charging.
* example Lovelace card (mushroom required).

# ToDo
Any contributions to improve the code are appreciated!
* Complete English translation (most entities have English descriptions in code)
* improve configuration
* improve accuracy
* sometimes the prediction fails by calculating negative percentages because of insufficient solar. this should be limited to realistic values (0-100%)
* use local weather data to improve prediction

# Installation
please contribute ANY upgrades to the card or algorithm this helps everybody!
1. copy all files oft the `battery-predict.yaml` into your custom yaml integrations folder
2. make changes appropriate to your setup (set entity IDs, battery size, average consumption...)
3. copy the card as a manual yaml config into Lovelace. !mushroom required!
4. edit the current production of solar entity in the conditional cards 

_

THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.
