# 9.-Design-and-Implementation-of-Astable-and-Monostable-Multivibrator
**Aim:**
To design and implement Astable-and-Monostable-Multivibrator-using-IC 555 Timer.

**APPARATUS REQUIRED:**
S.No	Name of the Apparatus	Range	Quantity
1.	Function Generator	3 MHz	1
2.	DSO	30 MHz	1
3.	Dual RPS	(0 – 30) V	1
4.	IC 555 timer	1
5.	Bread Board		1
6.	Resistors	10K,100K	2
7.	Capacitor	0.01µF,0.1 µF	Each 2
8.	Diode	1N4007	2
9.	Connecting wires and probes	As required	


**THEORY:**

**MONOSTABLE MULTIVIBRATOR**

A Monostable Multivibrator, often called a one-shot Multivibrator, is a pulse-generating circuit in which the duration of the pulse is determined by the RC network connected externally to the 555 timer. In a stable or stand by mode the output of the circuit is approximately Zero or at logic-low level. When an external trigger pulse is obtained, the output is forced to go high (  VCC). The time for which the output remains high is determined by the external RC network connected to the timer. At the end of the timing interval, the output automatically reverts back to its logic-low stable state. The output stays low until the trigger pulse is again applied. Then the cycle repeats. The Monostable circuit has only one stable state (output low), hence the name monostable. Normally the output of the Monostable Multivibrator is low.

 **ASTABLE MULTIVIBRATOR**

When the power supply VCC is connected, the external timing capacitor ‘C” charges towards VCC with a time constant (RA+RB) C. During this time, pin 3 is high (≈VCC) as Reset R=0, Set S=1 and this combination makes Q =0 which has unclamped the timing capacitor ‘C’.
When the capacitor voltage equals 2/3 VCC, the upper comparator triggers the control flip flop on that Q =1. It makes Q1 ON and capacitor ‘C’ starts discharging towards ground through
RB and transistor Q1 with a time constant RBC. Current also flows into Q1 through RA. Resistors RA and RB must be large enough to limit this current and prevent damage to the discharge transistor Q1. The minimum value of RA is approximately equal to VCC/0.2 where 0.2A is the maximum current through the ON transistor Q1.
During the discharge of the timing capacitor C, as it reaches VCC/3, the lower comparator is triggered and at this stage S=1, R=0 which turns Q =0. Now Q =0 unclamps the external timing capacitor C.  The capacitor C is thus periodically charged and discharged between 2/3
VCC and 1/3 VCC respectively. The length of time that the output remains HIGH is the time for
the capacitor to charge from 1/3 VCC to 2/3 VCC.

The capacitor voltage for a low pass RC circuit subjected to a step input of VCC volts is given by VC = VCC [1- exp (-t/RC)]
Total time period T = 0.69 (RA + 2 RB) C

f= 1/T = 1.44/ (RA + 2RB) C

**DESIGN: MONOSTABLE MULTIVIBRATOR**

Given Frequency F=1K Hz, T=1/F=1ms T=1.1RAC
Assume C=0.1µf, Find RA RA = T/1.1 C=10K

**DESIGN: MONOSTABLE MULTIVIBRATOR**

 Astable multivibrator of operation frequency = 1 KHz & duty cycle of 25% using 555 timer IC.
Given Frequency=1000Hz Duty cycle=25%
D= T low/T = RB/RA+2RB*100 100RB = 25(RA+2RB)
50RB – 25RA = 0	(1)
Given f=1KHz we know that T=1/f
T=1ms
T= T high + T low 0.69(RA+2RB)C = 1*10-3
0.69(RA+2RB) = 1*10-3/C Let C=0.1μF
0.69RA+1.38RB = 1*10-3/0.1*10-6
0.69RA+1.38RB = 10 4	(2)
Solving equation 1 & 2 we get
RA=7.2KΩ, RB= 3.6KΩ
 
**PROCEDURE:**

**MONOSTABLE MULTIVIBRATOR:**

1.	Connect the circuit as shown in the circuit diagram.
2.	Apply Negative triggering pulses at pin 2 of frequency 1 KHz.
3.	Observe the output waveform and measure the pulse duration.
4.	Theoretically calculate the pulse duration as Thigh=1.1. RAC
5.	Compare it with experimental values.

**ASTABLE MULTIVIBRATOR:**

1.	Calculate the value of R & C using design procedure.
2.	Connect the circuit as shown in the circuit diagram.
3.	Apply Negative triggering pulses at pin 2 of frequency 1 KHz.
4.	Observe the output waveform and measure the pulse duration.
5.	Theoretically calculate the pulse duration as T=1.1 RAC



  **CIRCUIT DIAGRAM**

<img width="998" height="1600" alt="image" src="https://github.com/user-attachments/assets/bedab084-e0c3-4f11-b250-af75bb1ea938" />


<img width="1005" height="1536" alt="image" src="https://github.com/user-attachments/assets/bf2729d2-96b5-4d86-888a-6e92f2a13fc4" />

 
<img width="1568" height="1600" alt="image" src="https://github.com/user-attachments/assets/e7fe45ec-e1be-401e-a3ac-99888eece3fa" />


<img width="899" height="1599" alt="image" src="https://github.com/user-attachments/assets/932a780e-22c8-4b8c-a4bb-15ff559cb1f5" />

<img width="1200" height="1600" alt="image" src="https://github.com/user-attachments/assets/b66d65e1-087a-4203-9461-13b6f9fd3c8a" />

**RESULT:**
Thus the Astable and Monostable multivibrator is designed and tested using 555 timer IC

 

