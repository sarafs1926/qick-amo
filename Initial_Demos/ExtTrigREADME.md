Hook up an AWG in pulse mode, e.g. a 10 ns long pulse set to 3.3 V height 0 V offset to trigger this, since the QICK tProc just needs an edge. 
Connect the AWG pulse output to the 2 PMOD pins specified in the below picture. The black lead is ground, the red lead is the pulse (low level 0 V, high level 3.3 V, rising edge trigger).

Now you are ready to try out the demo notebook ExtTrig.

![Image from iOS (1)](https://user-images.githubusercontent.com/22227509/175976840-deb603f9-e37c-468e-a33f-4cb21af10913.jpg)

During the test, if you do "acquire" with external triggering but you dont send a trigger you will see nothing and the tProc will just hang until a trigger is sent.
