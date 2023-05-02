Download Link: https://assignmentchef.com/product/solved-comp4336-9336-mobile-data-networking-phy-fundamentals-ii
<br>
Q1. Determine the received signal power observed by a user equipment (UE) at 4m and at a distance of 500 m from a 14 m high base station. The transmitter and receiver antenna gains are 10 dB and 5 dB, respectively. Transmitted power is 30 dBm. Do all calculations using dB.




A1.




PR = PTGTGRhT2hR2/d4

PR|dB = PT |dB + GT |dB + GR |dB + 10log10(hT2hR2/d4)

= 30 + 10 + 5 + 10 log<sub>10</sub>(14<sup>2</sup>*4<sup>2</sup>/500<sup>4</sup>) = 45 – 72.99

= -27.99 dBm




Q2. With a subcarrier spacing of 10 kHz, how many subcarriers will be used in an OFDM system with 8 MHz channel bandwidth?




A2.




Number of Subcarriers = (8×10<sup>6</sup>)/(10×10<sup>3</sup>) = 800







Q3. Let us consider an OFDMA system that uses the same carrier spacing irrespective of the channel bandwidth used. It employs 1024 subcarriers for 10 MHz channel. How many subcarriers will be used if the channel was (a) 1.25 MHz, (b) 5 MHz, (c) 8.75 MHz?




A3.




Inter carrier spacing = 10MHz/1024 = 9.7656 kHz

1.25 MHz = 1.25×10<sup>3</sup>/9.7656 = 128

5 MHz = 5×10<sup>3</sup>/9.7656 = 512

8.75 MHz = 8.75×10<sup>3</sup>/9.7656 = 896




Q4. If 100 mW transmit power is used by a 2.4 GHz WiFi router, find the received power in dBm at a distance of 20 meter (assume free space path loss with unit antenna gains).




A4.




P<sub>T</sub> = 100 mW = 20 dBm

G<sub>T</sub> = 1 = 0 dB

G<sub>R</sub> = 1 = 0 dB




P<sub>R</sub> for linear power units (mW/W): 0.0000247 mW




P<sub>R</sub> For logarithmic units (dBm/dBW): -46 dBm




Path       loss:     -­‐66    dB  Q5. Repeat the previous question for a 60 GHz WiFi router:




<ul>

 <li>what is the received power at 20 m?</li>

 <li>what transmit power should be used by the router if the same received power of Q4 was to be achieved at 20 m?</li>

 <li>at what distance the same received power of Q4 could be achieved if the router still used 100 mW?</li>

</ul>




A5.

<strong> </strong>

<ul>

 <li>952 x 10<sup>-8</sup> mW or -74 dBm</li>

 <li>60 GHz has 28 dB more path loss compared to 2.4 GHz. This excess path loss can be adjusted by increasing the transmit power by 28 dB. The required power in 60 GHz = power in 2.4 GHz + 28 dB, i.e. 20 dBm+28 = 48 dBm (note that 100mW = 20 dBm).</li>

 <li>Q4 has a received power of -46 dBm. Given that the transmit power is 20 dBm, we can only tolerate a path loss of 66 dB. At 60 GHz, 66 dB is lost just at 80 cm distance!</li>

</ul>




Q6. You have bought a 2.4 GHz WiFi router with two dipole antennas claiming effective antenna gain of 6 dB. Your laptop has a single dipole with 0 dB gain and it claims a receiver sensitivity of -64 dBm. Calculate the maximum distance from the router your laptop can receive data if the router always use a transmit power of 20 dB.




A6.




We can tolerate a maximum pathloss of 90 dB (20+6+64 = 90). 2.4 GHz will lose 90 dB at 315 m. Beyond 315 m from the router, the laptop will receive signal strength below its sensitivity level and hence will not be able to decode information.




Q7. You have bought a 2.4 GHz WiFi router with antenna gain of 6 dB and default transmission power of 100 mW. Your laptop has a 0 dB antenna gain and claims a receiver sensitivity of -60 dBm. Can you connect your laptop to the router from a distance of 150 m? Why or why not?




A7.




There is 83.56 dB path loss at 150 m. Therefore the laptop will receive a signal strength of 20+6-83.56 = -57.56 dBm, which is higher than its receiver sensitivity. Therefore the laptop can connect to the router.




Q8. What degrees of freedom we have for the following MIMO configurations:




<ul>

 <li>2×2 MIMO</li>

 <li>4×2 MIMO</li>

 <li>10×4 MIMO</li>

 <li>20×10 MIMO</li>

 <li>20×20 MIMO</li>

</ul>







A8.




<ul>

 <li>Degrees of freedom = min(2,2) = 2</li>

 <li>Min(4,2) = 2</li>

 <li>Min(10,4) = 4</li>

 <li>Min(20,10) = 10</li>

 <li>Min(20,20) = 20</li>

</ul>




Q9. Inspired by the MIMO technology, you are committed to design new laptops with lots of antenna elements fitted to it. For a linear (1 dimensional) antenna array, how many antennas can you fit within a length of 15 cm for the following WiFi bands?




<ul>

 <li>4 GHz</li>

 <li>8 GHz</li>

 <li>60 GHz</li>

</ul>




A9.




<ul>

 <li>λ = c/f = 3×108/2.4×109 = 12.5 cm. For at least λ/2 antenna separation, we can fit at most 3 antennas within 15 cm.</li>

 <li>λ for 5.8 GHz = 5.17 cm. We can fit 6 antennas within 15 cm. (c) λ for 60 GHz = 0.5 cm. we can fit 61 antennas within 15 cm.</li>

</ul>




Q10. In future, we may be forced to use frequencies as high as 10 THz to transmit data superfast required for some yet-to-be invented applications. What size of antenna (full length) would we need for such devices?




A10.




End-to-end antenna length = λ/2. λ for 10 THz = 29.98 µm

We there for need very small antennas of size less than 15 µm!











