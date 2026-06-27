# 8hp VCO/LFO

![](https://github.com/Fihdi/UNO/blob/main/UNOFront.png?raw=true)

UNO (Universal Oscillator) is an all-purpose voltage controlled oscillator / LFO. The frequency range can be switched from low (**LFO** mode) to high (**VCO** mode).

The frequency of the oscillator can be set by the **FREQ** knob as well as the **V/O** input, **FM** input and **FM** knob. 

The **PWM** input can change the duty cycle of the **SQR** output. Its is possible to achieve 0% or 100% duty cycle, giving the user the ability to stop the oscillation of the **SQR** output.

The **SUB** output creates a square wave with half the frequency of the **SQR** signal, 

The **IN** input overrides the oscillator completely and turns UNO into a slew rate limiter. The Triangle output follows the **IN** input with the speed set by the **FREQ** knob as well as the **V/O** and **FM** CVs.

The **SYNC** input is a less extreme version of the **IN** input. Instead of overriding, it creates an average between the **SYNC** and the oscillator signal. By varying the strength of the **SYNC** signal it is possible to go from soft- to hard-synchronization.

The **U/D** (Up/Down) output is 5V when the **TRI** output is rising and -5V when **TRI** output is falling. NOTE when using UNO as a slew rate limiter: When the **TRI** output has reached the **IN** input, the **U/D** output starts to oscillate wildly.

**SIN** is a sinusoid version of **TRI**. The **SAW** output is twice the frequency of **TRI** and **SIN**.

Switching the module to **ENV** and sending a rising edge to the **TRG** input makes the **TRI** output go from 0V to 8V and back to 0V.

A trimmer on the back of the module can be used to tune the volt per octave tracking. 
