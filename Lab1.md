Author  : Phan Minh Anh

Email   : <anhphan21@outlook.com>

Date    : December, 2021

# Lab 1-EE331 tutorial

__Getting started with LTSPICE__: [link](http://www.simonbramble.co.uk/lt_spice/ltspice_lt_spice.htm)

## Procedure 1

```Aim```: Measure the  leakage current of 2 kinds of diode.

```Object```: ~~1N34A~~, 1N4007, 1N5819.

How to add custom component into LTSPICE: [link](https://www.analog.com/en/education/education-library/videos/5579239882001.html)

Model for component:
- 1N4007:   
> .model 1N4007 D(IS=7.02767n RS=0.0341512 N=1.80803 EG=1.05743 XTI=5 BV=1000 IBV=5e-08 CJO=1e-11 VJ=0.7 M=0.5 FC=0.5 TT=1e-07 mfg=OnSemi type=silicon)

## Procedure 2

```Aim```: Measure the turn on voltage of diode

```Object```: ~~1N34A~~, 1N4007, 1N5189.

Set up:
    
    R1  = ????
    D1  = 1N4007, 1N5189
    VSS = 0V - 11V

Hint: Using .dc sweep to run the simulation

## Procedure 3

```Aim```: Plot I-V characteristic of diode

```Object```: ~~1N34A~~, 1N4007, 1N5819.

Set up:

    R1  = ????
    D1  = 1N4007, 1N5819
    VSS = 0V - 11V

Hint: Using .dc sweep to run the simulation

# Procedure 4

```Aim```: Plot I-V characteristic of diode

```Object```: ~~1N34A~~, 1N4007, 1N5819.

# Procedure 5

```Aim```: Plot I-V characteristic of diode

```Object```: 1N4732

Library for Zenner diode 1N4732: [Link](http://www.simonbramble.co.uk/lt_spice/ltspice_lt_spice_models.htm)
