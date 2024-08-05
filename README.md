# Upcounter-Cadence Virtuoso
Schematic and simulation of 4-bit Asynchronous Upcounter.

The upcounter is built using four D-flipflops(Master-slave configuration) .
 It is 
capable of counting numbers from 0 to 15.

The D-flipflop in this project is created using D-latches which is created by user built nand-gates and inverters.
D-Flip flop being edge-triggered and D-Latch being level-triggered. 
Latches work on master-slave principle with the inverted clk given to the 
second latch.

Diagram of D-flipflop:
![image](https://github.com/RakeshpatilLB/Cadence-Upcounter/assets/167572033/bb72f7da-37a1-48ff-abf7-b7359871c7a5)

Working of Master-slave D-flipflop:

When “clk=0”, Master D-Latch is Transparent, whereas Slave D-Latch is Opaque. 
When D=0, the output of the master latch is Zero and the output of slave latch is 
the previous value.
When “clk=1”, Slave D-Latch is Transparent, whereas Master D-Latch is Opaque. 
The data D which was transmitted from Master D-Latch is observed in the output 
irrespective of D.

i.e, the D-Flip flop becomes transparent (i.e allows the data 
D to pass through it) during rising edge of the clk and becomes opaque (i.e does 
not allow the data D to pass through it/retains the previous value) until the next 
rising edge.



D-flipflop schematic in Cadence-virtuoso:
![image](https://github.com/RakeshpatilLB/Cadence-Upcounter/assets/167572033/11a93e6c-8551-4ba0-b97b-a878551cea81)

Symbol:
![image](https://github.com/RakeshpatilLB/Cadence-Upcounter/assets/167572033/c929bc98-74a3-4b1a-a716-e64925ff13d3)

Schematic of Asynchronous-Upcounter:
![upcounetrsch](https://github.com/RakeshpatilLB/Cadence-Upcounter/assets/167572033/5bb0b493-d0dc-4989-9eca-54a5b76963a8)

Simulation Results:
![upcountersim](https://github.com/RakeshpatilLB/Cadence-Upcounter/assets/167572033/0fd20e90-3394-488c-99bf-e2bdf66c90a0)

Delay Estimation Clock to Q:
![delay](https://github.com/RakeshpatilLB/Cadence-Upcounter/assets/167572033/90bb02ab-f119-4b4f-952f-1c90a96ac560)

average delay=(94.033a+130.305)/2
             =112.16 ps.


Conclusion:

In conclusion, the development of an asynchronous upcounter circuit using D 
flip-flops showcases an innovative approach to designing efficient and reliable 
sequential circuits. This design not only reduces power consumption and 
improves speed but also offers flexibility and scalability. The successful 
implementation of this project can pave the way for various applications in 
digital systems, contributing to the advancement of modern technology.


Applications:

Asynchronous Up Counters designed using D flip-flops are used in 
applications such as : Timing and synchronization, pulse generation and 
counting, data transmission and communication and etc.


                                                            THANK YOU!

      




