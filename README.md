java c
EE3C, Power Electronics and Power Systems 
Assignment on Power Electronics, 2024-25 
Task 1 (Marks: 20) A   three-phase   6-pulse   diode   rectifier,   connected   to   a   3-phase   AC   supply,   having   a   voltage   of   415   V   (line-to-line   RMS),   a   frequency   of   50 Hz,   and   a   per   phase   series   inductance of Ls = 5mH, feeds   a   static RL load.
Question 1 
Draw the circuit diagram of   the   AC-DC diode converter.                                                                                                          [2]
Question 2 Implement   this   rectifier   in   Simulink.   The   diodes   have   a   forward   voltage   drop   of   1.0 V when conducting. Model the load as the series   of   a resistor R   =   10   Ω   and   an   inductor L =   100 mH.
Question 3 
Using   the   circuit   parameters   of   Question   2:
Task 2 (Marks: 40) A   three-phase 6-pulse, fully controlled thyristor rectifier supplies a static RL load, from   a   three   phase   415 V   (line-to-line   RMS),   50 Hz, AC   supply   having   a   per   phase   series   inductance   of Ls = 2.5 mH.
Question 1 
Draw the circuit diagram of   the   AC-DC thyristor converter.                                                                                     [2]
Question 2 Implement this rectifier in Simulink. The thyristors have a forward voltage drop of 1.0   V   when    conducting.    Model   the   load    as   the    series    of   a    resistor R and an inductance L.
Investigate the following cases in the simulation   study:
a) R = 50 Ω, L = 2 mH   andLs =   2.5 mH;
b) R = 50 Ω, L = 200 mH   andLs = 2.5 mH;
c) R =   10 Ω, L = 200 mH   andLs = 2.5 mH;
d) R =   10 Ω, L = 200 mH andLs =   10 mH.
For all cases,   the firing angle of   thyristors   has   to   be chosen   to get an average voltage   of   500 V across the load.
In   your   report,   you    have    to    show    and    comment    (maximum    2    sentences)    the   following for all the   cases:
1.          the firing angles to achieve the desired   load voltage;                                                                   [1+1+1+1]
2.          the waveforms of   the DC voltage across the load;                                                                               [2+2+2+2]
3.          the   values   of   the   THD   of   the   currents   of   the   three   phase   AC   supply;    [1+1+1+1]
4.          the power factor   seen by the AC   supply, remembering   that   the   voltage
is sinusoidal but the current is distorted.                                                                                                                               [2+2+2+2]
Question 3 
Using the rectifier model of   Question 2 and assuming Ls = 2.5   mH, R =   50   Ω,   and L = 200   mH:
Task 3 (Marks: 40) 
A   pulse-width   modulated   (PWM)   three-phase   inverter,   shown   in   Fig.   1,   supplies   a   three-phase, Y-connected static RL load, connected to the nodes A, B, C. The input DC   voltage Vd is smooth and equal   to   600   V.

Fig.   1. Three-phase inverter supplying a static   RL load
Question 1 Develop   a   Simulink   model   for   the   inverter,   using   IGBT   as   power   devices   and   sinusoidal    PWM    with    triangular    carrier    as    a    modulation    technique.    The    load   parameters      are R = 25 Ω       and L = 200 mH.       The      modulation       frequency      and   amplitude   ratios are mf = 9 and ma = 0.8, respectively. For a fundamental frequency   of   the   output voltage   of   25 Hz   and with reference to   the   circuit   in   Fig.   1,   show   in   the report:
Question 2 
The inverter is modulated with a   sinusoidal   PWM with   triangular   carrier. Assume R = 25 Ω, L = 50 mH, ma = 0.8 and   fundamental   frequency   output   of   25 Hz.
1.       Design the   value of   the frequency   ratio mf to keep the   THD of   the output current below 2%.                                                               [10]
2.       Verify your design using your computer simulation.                                                                                                          [6]
Question 3 
The inverter is modulated with a   sinusoidal PWM   with   triangular   carrier. Assu代 写EE3C, Power Electronics and Power Systems Assignment on Power Electronics, 2024-25Matlab
代做程序编程语言me R = 25 Ω, L = 50 mH, mf = 31 and fundamental   frequency   output   of   25   Hz.
Remarks 
These   instructions have been tested   in Matlab   2023a.   Other Matlab   versions   might   be slightly different.
1)         Remember to add units and titles to all diagrams included   in the   report.
2)         A simple way to improve the legibility of   the figures it to change the settings of   the   scopes:
a.          Click    on    “view”,   “Configuration   properties”,   “Time”,   to   add   the   time-axis   label and select the   x-axis   unit
b.          Click   on “view”, “Configuration   properties”, “Display”, to   add   they-axis   unit   and the title;
c.          Click on “view”,   “Style”   will   enable   you   to   change   the   background   colour   of   the figure, the linewidth and   colour of   the   lines.
3)          Some      Simulink    examples    of   AC-DC      converters      and      DC-AC      converters      are   available on   Canvas.
4)         Use the tutorial notes for Simulink and Matlab to help you   for   the   development   of the simulations.
5)          Starting   from   the   example   for   three-phase   diode   rectifier,   change   the   diodes   to   thyristors.   The   thyristors   can   be   controlled   by   the   “Pulse   generator   (Thyristor   6-   pulse)”, placed in “Simscape”, “Electrical”, “Specialized Power Systems”, “Power   Electronics”, “Power Electronics Control”   .   Alternatively, you can search the block   from   the   search   bar   at   the   top   of   the “Simulink   Library   Browser”   .
6)         The   frequency   of   synchronisation   (input   “wt”)   can   be   obtained   with   3-phase   a      phase-locked   loop   algorithm,   block   “PLL   (3ph)”   from   the AC   power   source. An      angle duration of 10 degrees is often enough to turn the thyristors on.   A “constant”   block can feed the input “block”, putting the constant   equal to zero.
7)         A   good    example    of   a    6-pulse    controlled    rectifier    can    be    found    by    typing    in   “power_ThyristorRectifiers” in   the   main   Matlab   window.
8)         The “PWM generator (2-level)” block can be found in the same folder of   the pulse      generator   forthyristors. Change   the   generator   mode   to “3-phase   bridge   (6 pulses)”   and   tick “internal   generation   of   reference   signal”   .
9)         To   change the resistance   as   a   step, you   can use two   resistors   in   parallel,   with   one   of   the    two   resistors    series    connected    to    an    ideal    switch    (“Specialized    Power systems”,   “Power   Electronics”). The   switch   is   open when the   input   “g”   is   0,   it   is   closed when “g” is   1. The switch   is   initially   open,   so   only   one   of   the two   resistors   is   connected   to   the   rest   of the   circuit   (e.g.   50   Ω).   When   the   switch   is   closed   by   changing   the   input   to   port   “g”   from   0   to    1,   the   second   resistor   is   connected   in   parallel,   reducing   the   total   load   resistance.   For   example,   if the   second   resistor   is 33.3 Ω and the first resistor is 50   Ω, the   equivalent   resistance   is   20   Ω   .
10)   PID   controller blocks   are   already   available   in   Simulink   in   the   folder   “Simulink”,   “Continuous”   .    These      controllers      have      all      the      functions      already      implemented,   including   saturation   and   anti-windup.
11)   PID controllers work for the control of   both DC and   AC   quantities.
12)   To control a quantity “x”, you   need   to   see   “x”   as   the   effect   and you   have   to   adjust   the quantity “y”, where “y” is   the   cause   of “x”   . For   example,   in   an   electric   circuit   the   current   is   the   effect   and   the   voltage   is   the   cause;   if you   want   to   control   the   current,   you   have   to   regulate   the   voltage.   Therefore,   the output of   the   PID controller   is the voltage reference that is generated by the converter.
13)   In the model answers, the number of   sentences is indicative of   the expected length   of   each answer and it   is not prescriptive.




         
加QQ：99515681  WX：codinghelp  Email: 99515681@qq.com
