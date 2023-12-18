 up counter and down counter 
### AIM: To implement 4 bit up and down counters and validate  functionality.
### HARDWARE REQUIRED:  – PC, Cyclone II , USB flasher
### SOFTWARE REQUIRED:   Quartus prime
### THEORY 

![Screenshot 2023-12-18 210223](https://github.com/Kathiresan-23013376/Exp-7-Synchornous-counters-/assets/150008375/f52e0f6f-ac99-4dd5-ab5d-a442d12afef0)


## UP COUNTER 
The counter is a digital sequential circuit and here it is a 4 bit counter, which simply means it can count from 0 to 15 and vice versa based upon the direction of counting (up/down). 



![Screenshot 2023-12-18 210233](https://github.com/Kathiresan-23013376/Exp-7-Synchornous-counters-/assets/150008375/1f8104e3-8984-4f10-b8ed-2a9564a6098b)

 



The counter (“count“) value will be evaluated at every positive (rising) edge of the clock (“clk“) cycle.
The Counter will be set to Zero when “reset” input is at logic high.
The counter will be loaded with “data” input when the “load” signal is at logic high. Otherwise, it will count up or down.
The counter will count up when the “up_down” signal is logic high, otherwise count down

Since we know that binary count sequences follow a pattern of octave (factor of 2) frequency division, and that J-K flip-flop multivibrators set up for the “toggle” mode are capable of performing this type of frequency division, we can envision a circuit made up of several J-K flip-flops, cascaded to produce four bits of output.
The main problem facing us is to determine how to connect these flip-flops together so that they toggle at the right times to produce the proper binary sequence.
Examine the following binary count sequence, paying attention to patterns preceding the “toggling” of a bit between 0 and 1:
Binary count sequence, paying attention to patterns preceding the “toggling” of a bit between 0 and 1.

Note that each bit in this four-bit sequence toggles when the bit before it (the bit having a lesser significance, or place-weight), toggles in a particular direction: from 1 to 0.


![Screenshot 2023-12-18 210400](https://github.com/Kathiresan-23013376/Exp-7-Synchornous-counters-/assets/150008375/c7652be1-6d92-4fbf-8875-ac555ac2ed23)


![Screenshot 2023-12-18 210410](https://github.com/Kathiresan-23013376/Exp-7-Synchornous-counters-/assets/150008375/1b4c33c7-8fda-48b6-8ada-7a9091166fcd)

Starting with four J-K flip-flops connected in such a way to always be in the “toggle” mode, we need to determine how to connect the clock inputs in such a way so that each succeeding bit toggles when the bit before it transitions from 1 to 0.

The Q outputs of each flip-flop will serve as the respective binary bits of the final, four-bit count:

 
 

Four-bit “Up” Counter
![image](https://user-images.githubusercontent.com/36288975/169644758-b2f4339d-9532-40c5-af40-8f4f8c942e2c.png)



## DOWN COUNTER 

As well as counting “up” from zero and increasing or incrementing to some preset value, it is sometimes necessary to count “down” from a predetermined value to zero allowing us to produce an output that activates when the zero count or some other pre-set value is reached.

This type of counter is normally referred to as a Down Counter, (CTD). In a binary or BCD down counter, the count decreases by one for each external clock pulse from some preset value. Special dual purpose IC’s such as the TTL 74LS193 or CMOS CD4510 are 4-bit binary Up or Down counters which have an additional input pin to select either the up or down count mode.
 
 ![Screenshot 2023-12-18 210350](https://github.com/Kathiresan-23013376/Exp-7-Synchornous-counters-/assets/150008375/172a9d9a-2500-448c-9168-41320c0da4d9)

![Screenshot 2023-12-18 210400](https://github.com/Kathiresan-23013376/Exp-7-Synchornous-counters-/assets/150008375/ec73624d-43ff-489d-9a46-881676452608)


![Screenshot 2023-12-18 210410](https://github.com/Kathiresan-23013376/Exp-7-Synchornous-counters-/assets/150008375/f986a98e-bbde-451c-a21f-bf0abaf65806)



4-bit Count Down Counter
### Procedure
/* write all the steps invloved */



### PROGRAM 
/*
Program for flipflops  and verify its truth table in quartus using Verilog programming.
Developed by: Kathiresan-K
RegisterNumber: 23013376
*/

### TRUTH TABLE 

![download](https://github.com/Kathiresan-23013376/Exp-7-Synchornous-counters-/assets/150008375/fc223bf6-9083-4e34-882e-dd6e29495d6d)


![download](https://github.com/Kathiresan-23013376/Exp-7-Synchornous-counters-/assets/150008375/b2a6088e-5e38-4e84-98a2-f03547254925)





### RESULTS 
