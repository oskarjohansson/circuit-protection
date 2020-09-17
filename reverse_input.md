# Reverse input

> Created by Oskar Johansson
>
> Gathered from: https://www.electronicdesign.com/power-management/article/21801509/reversepolarity-protection-in-automotive-design
>
> Infineon application note: https://www.infineon.com/dgdl/Reverse-Batery-Protection-Rev2.pdf?fileId=db3a304412b407950112b41887722615

If the power input has a possibility to be reversed, a protection is a good idea. 

## Simple P-mosfet

![](C:\Users\oskar\Dropbox\Dokument\Projekt\circuit-protection\img\reverse_pmos.PNG)

The simple P-Mosfet is useful if the circuit doesn't need to handle high currents and want the most simple solution. The body diode will first conduct current when connected and then the mosfet will switch on. 

## Simple N-mosfet

![](C:\Users\oskar\Dropbox\Dokument\Projekt\circuit-protection\img\reverse_nmos.PNG)

The simple N-mosfet is useful if you don't have a common ground with your power supply. If the load is a unit among others, not having a common ground may cause problem. Otherwise this would be cheaper than the solution with the P-mosfet. 

## Simple Ideal diode

![](C:\Users\oskar\Dropbox\Dokument\Projekt\circuit-protection\img\reverse_ideal.PNG)

By combining the best of having a N-mosfet and having a common ground, an ideal diode circuit can solve that. LM74610-Q1 or LM74700Q is example of that kind of circuit. 



