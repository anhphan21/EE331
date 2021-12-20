Author  : Phan Minh Anh

Email   : <anhphan21@outlook.com>

Date    : December, 2021

# __Lab 1 - EE331 tutorial - Operation of Diode__

__Getting started with LTSPICE__: [link](http://www.simonbramble.co.uk/lt_spice/ltspice_lt_spice.htm)

## __Procedure 1__

```Aim```: Measure the  leakage current of 2 kinds of diode.

```Object```: 1N4007, 1N5819.

```Hint```:

How to add custom component into LTSPICE: [link](https://www.analog.com/en/education/education-library/videos/5579239882001.html)

Model for component:
- 1N4007:   
> .model 1N4007 D(IS=7.02767n RS=0.0341512 N=1.80803 EG=1.05743 XTI=5 BV=1000 IBV=5e-08 CJO=1e-11 VJ=0.7 M=0.5 FC=0.5 TT=1e-07 mfg=OnSemi type=silicon)

```Measurement```: Measure leakage current of 2 diodes

```Question```: 
* Compare leakage current of 2 diodes.
* Which diode is the most suitable for charging capacitor.

## __Procedure 2__

```Aim```: Measure the turn on voltage of diode

```Object```: 1N4007, 1N5189.

```Hint```:

Set up:
    
    R1  = 100, 1k, 10k, 100k, 1M, 10M
    D1  = 1N4007, 1N5819
    VSS = 10V

Using .param to save your time

```Measurement```: Turn on voltage of 2 diodes

```Question```: 
* Plot I-V graph of diode (I axis in log 10 scale, V axis in linear scale)
* Slope of each diode
* Rank turn on voltage of diode and compare to leakage current

## __Procedure 3__

```Aim```: Plot I-V characteristic of diode

```Object```: 1N4007, 1N5819.

```Hint```:

Set up:

    R1  = 1k
    D1  = 1N4007, 1N5819
    VSS = 0V - 11V

Using .dc sweep to run the simulation

```Measure```: I-V characteristic

```Question```: Compare Von to procedure 2

# __Procedure 4__

```Aim```: Effect of series and parallel resistances

```Object```: 1N4148

```Measure```:
* I-V characteristic of original 1N4148
* I-V characteristic of 1N4148 with parallel res
* I-V characteristic of 1N4148 with serial res

```Question```: Discuss the effects of series and 
parallel resistance on the observed I-V characteristics of a diode.

# __Procedure 5__

```Aim```: Plot I-V characteristic of diode

```Object```: 1N4732

Library for Zenner diode 1N4732: [Link](https://www.opel.ece.vt.edu/reference/datasheets.html)

```Measure```: I-V characteristic of original 1N4732

```Question```:
* Compute Rz of 1N4732
* Calculate maximum current of diode in forward