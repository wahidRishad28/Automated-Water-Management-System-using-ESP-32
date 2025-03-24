# Automated-Water-Management-System-using-ESP-32

#Software used-
1. Arduino IDE
#Hardware used-
 1. Arduinomega
 2. PumpX2
 3. RelayX2
 4. MiniWaterTank
 5. Miniwatertank(reserve)
 6. Powersupply(12v,5v)
 7. Esp32developmentboard
 8. Waterlevelsensor
 9. Waterqualitysensor
 10.Screen/Ledmonitor
 11.Wires
 12.Alarm(Buzzer)
 13.Switch
 14.PushButton
 15.Wires
# This working method for various features :
 1. Water level control and alarm : When the water is below certain level, an alarm will
 ring and notify the user and then automatically pump and fill the tank to a set level. It
 utilizes a water level sensor, which will be connected with arduino through the analog
 pins. The motor(pump) will be controlled by a 5v relay. The pump itself will operate with
 12v DC power supply.
 2. Integration with weather : The project uses esp32 board which will be connected to
 nearby wifi and it will fetch weather "Precipitation" data from a weather api, which will be
 fed to the arduino. The arduino will monitor the rate or water decreasing and according
 to set algorithm, it will not fully fill the water tank if there is an upcoming rain, instead it
 will calculate rain duration and fill the tank accordingly.
 3. Useabandoned rain water in a reserve tank : Abandoned rain water will be collected
 in a reserve tank and will be used to wash cars or other works where water quality is not
 the most important thing.
 4. Water quality monitor : The tank may accumulate various dirt and the water quality
 may degrade over time. This project will use a TDS meter to monitor water quality and
 notify the user to clean the water.
