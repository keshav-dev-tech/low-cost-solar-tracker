# Electronics
- Voltage(volts): it is a force that pushes charged electrons through a conducting loop. More voltage means more pressure which means more electrons are pushed.
- Voltage is equal to the difference in electrical potential energy from 2 points in a circuit.
- Current(amps): while voltage pushes electrons into motion(pressure), current is the physical movement of electrical energy.
- So, voltage means the electrical pressure that pushes electrons and current is like the electricity flow rate, it represents the movement electrical energy.
- There are 2 types of current.
- Direct Current(DC): electricity flows in only 1 direction type of power supplied mostly by batteries as well as solar cells(important for this)
- Alternating Current: Electricity reverses direction periodically back and forth(type of power delivered to homes through wall outlets.
- 1 amp represents about 6.24 quintillion electrons moving past a single point every second.
- Resistance: resistance is the opposition to the flow of current. It's like friction that slows down the movement of electrons in a circuit. It goes against current.
- Materials can have different types of resistance(insulators and conductors).
- Insulators are materials that block current(movement of electrons) easily while conductors are materials that let current pass easily/have low resistance.
- Resistance(Ohms) measures how hard it is for electrical current to pass through a certain material.
- Different components of an electronic system are supposed to have a certain amount of resistance so that the circuit works properly.
- All these 3 things including continuity(testing if current can flow through the circuit) can be measured using a digital multimeter.
- https://www.youtube.com/watch?v=TdUK6RPdIrA This video is really helpful to learn how to use a multimeter.
- Ohm's law: electrical current flowing through a circuit is directly proportional to the voltage pushing it and inversely proportional to the resistance blocking it.
- Formula: I = V/R
- Resistor: a tiny electronic component meant to resist or slow down the electrical current.
## Voltage Dividers
- A voltage divider is a simple and fundamental circuit that scales down a high voltage to a lower one.
- It takes the incoming voltage and divides it using a pair of resistors connected in series.
- It starts with Vin(voltage in) and then goes downhill and fights through resistor 1 and then fights through resistor 2 and then by the time the current fights through both those resistors, the voltage would be around 0.
- The Vout is taken from the middle of the 2 resistors because, if it is taken after the 2 resistors, than the voltage will be around 0.
- Formula for Vout: Vout = Vin * (R2/(R1 + R2))
## LDRs
- LDRs are Light Dependent Resistors or photoresistors.
- They are electronic components where their resistance changes based on the amount of light shining on it.
- More light = less resistance while less light = more resistance.
- Voltage dividers are the essential bridge that allow LDRs to talk to a computer chip.
- Since microcontrollers/arduino only measures can't read resistance directly(they can only measure voltage), By using the formula for Vout, you can get the amount of voltage for resistor 1 rather than resistance.
## Analog vs Digital Signal
- In analog signal, it copies nature where things change gradually.
- analog signals can read a smooth or continuous slide of voltages between 0V and whatever amount of volts.
- When analogRead is used in Arduino, it slices the voltage into a number between 0 and 1023 and based on were its located between 0 and the target number of volts, it will spit out a number that is between 0 and 1023 that represents where it is located between 0 and target number of volts.
- However when digitalRead is done when using Arduino, it doesn't care how much volts is there or where its located between the interval. If it is higher than a certain number on the internal, it spits out 1 while if its not, it spits out 0.
-  
