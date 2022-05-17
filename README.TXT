The folder contains the Tip RGB models described in the following paper:
Saltas & Tognelli, 2022, MNRAS, in press (arXiv: 2203.02499)

There are two zip files:

1) TRGB_AllZ_theo.tar.bz2
2) TRGB_AllZ_photometry.tar.bz2

which contain the models for several values of teh total metallicity/helium.
There are 14 values for the couple (Z,Y), namely,

(Z,Y) = (0.0001,0.2472)
(Z,Y) = (0.0002,0.2474)
(Z,Y) = (0.0004,0.2478)
(Z,Y) = (0.0006,0.2482)
(Z,Y) = (0.0008,0.2486)
(Z,Y) = (0.0010,0.2490)
(Z,Y) = (0.0020,0.2510)
(Z,Y) = (0.0040,0.2550)
(Z,Y) = (0.0060,0.2590)
(Z,Y) = (0.0080,0.2630)
(Z,Y) = (0.0100,0.2670)
(Z,Y) = (0.0130,0.2730)
(Z,Y) = (0.0160,0.2790)
(Z,Y) = (0.0200,0.2870)

TRGB models have been computed for the reference set of parameters/input physics as described in the quoted paper. Each file contains 25 values of the stellar mass from 0.8 to 1.4 Msun, in steps of 0.025 Msun.
The details for each file are given below.

----------------------
TRGB_AllZ_theo.tar.bz2
----------------------
It contains all the theoretical quantities for TRGB model. Each file has the following format:

TRGB_Z0.xxxxx_He0.xxxxx_ML2.0000_OV0.000_CF11a0_NEW.DAT

where Z0.xxxxx is the overal metallicity and He0.xxxxx is the helium mass fractional abundance. 

Each file contains 12 columns,with the following quantities:
 1  NMD       : integer
 2  log t(yr) : float, log10 of the age at the TRGB (in years)
 3  log Teff  : float, log10 of the model effective temperature (in K)
 4  log L/Ls  : float, log10 of the model luminosity (in solar units)
 5  Mc(He)    : float, mass of the central helium core (in solar mass)
 6  Xc        : float, central hydrogen abundance (mass fraction)
 7  M/Ms      : float, actual value of the stellar mass at the tip
                (in solar mass)
 8  log g     : float, log10 of the surface gravity (in cgs)
 9  Ys        : float, surface helium abundance (mass fraction) at the TIP
10  Zs        : float, surface metallicty (mass fraction) at the TIP
11  [Fe/H]    : float, surface [Fe/H] value at the TIP
12  Mtot/Ms   : float, initial value of teh stellar mass (in solar mass)

----------------------------
TRGB_AllZ_photometry.tar.bz2
----------------------------
It contains the magnitudes in several bands. The file name is similar to that of the previous set of files. In addition it contains the name of the photometric system, which can be:
"UBVRIJHKLM"       : Johnson/Cousins magnitudes
"2MASS"            : 2MASS magnitudes
"GBpRpRVs_EDR3"    : Gaia eDR3 magnitudes
"WFC3"             : Wide Field Camera 3 magnitudes

Each file contains a variable number of columns which depends on the number of filters in the specific system. The first 6 columns are the same in each file as they list the following quantities:

1 Mini/Ms  : initial mass (in solar mass)
2 M/Ms     : mass at the TIP (in solar mass)
3 log t    : log10 stellar age at the TIP (in years)
4 log L/Ls : log10 stellar luminosity at teh TIP (in solar luminosity)
5 log Te   : log10 stellar effective temperature at the TIP (in K)
6 [Fe/H]   : surface [Fe/H] at the TIP

The other columns list the absolute magnitude in each photometric band.
