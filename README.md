# NUS-TEE2028-EE2028
This project was done by me and my partner, Low Feng Rui in fulfillment of the requirements for NUS TEE2028 (Microcontroller Programming and Interfacing) module in AY21/22 Sem 1<br><br>
This project is about implementing a system which does enhanced monitoring of COVID19 patients, especially elderly patients. This system is referred to as COvid Patients Enhanced MONitoring(COPEMON) and utilises various sensors on the board for data capture and transmission to an IoT server known as CHIP Associated Clou Unit(CHIPACU).

COPEMON has two modes of operation; Normal and Intensive Care(ICU) mode. Under each mode, COPEMON will capture data using different sensors and transmit to CHIPACU if certain conditions are met. 

<b>Sensor Usage and Potential Implementations</b> <br>
- <b>Accelerometer</b> <br>
Monitors the posture of the patient, specifically for fall detection.<br> 
- <b>Magnetometer(only in ICU mode)</b><br>
Monitors the orientation of the patient lying on the bed. Proper orientation is important in ensuring that other monitoring / life-saving equipment remains connected properly.
- <b>Pressure Sensor</b><br>
Simulates the pressure of air in the patient's lungs. A change in pressure can be varied by varying the height at which the sensor is held. 
- <b>Temperature Sensor</b><br>
Monitor body temperature. 
- <b>Humidity Sensor</b><br>
Measures the relative humidity of the air passed into the patient's lungs.
- <b>Gyroscope (only in ICU mode)</b><br>
Measures patient's movement; specifically to sense the patient's sudden twisting/twitching which could be an indication that the patient is in pain. A sudden movement can also cause issues with the other monitoring / life-saving equipment such as ventilators


To ensure safety and well-being of the patients, threshold values have been set for each of the sensors to differentiate if the patient is well or requires medical attention. Should there be any threshold crossing detected, COPEMON will transmit warning messages to CHIPACU to alert the relevant personnel.
