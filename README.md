Laser Security Alarm System (Hardware-Based)
Project Overview
This project is a simple yet effective laser-based security system. It uses an LDR (Light Dependent Resistor) and a BC547 NPN Transistor to trigger a buzzer when a laser beam is interrupted.


Component,Specification,Quantity
Transistor,BC547 (NPN),1
Sensor,LDR (5mm),1
Alarm,5V - 9V Active Buzzer,1
Resistor,10k$\Omega$,1
Power Source,9V Battery / DC Supply,1
Laser,5V Red Laser Diode,1

From Component,    Pin/Terminal,     To Component,      Pin/Terminal
BC547              Emitter           Battery            Negative (-)
BC547              Base              LDR                Pin 1
BC547              Base          10k$\Omega$ Resistor   End A
10k$\Omega$ Resistor,End B       Battery              Positive (+)
LDR,              Pin 2          Battery             Negative (-)
Buzzer          Positive (+)      Battery             Positive (+)
Buzzer          Negative (-)     BC547                Collector
