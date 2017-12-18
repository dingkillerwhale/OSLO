# OSLO
Optics Software for Layout and Optimization


CCL notes

- Spreadsheet Buffer

it is an array of numerical storage cells with 1999 rows numbererd as in Mocrosoft Excel and 10 columns numbered as a, b c, d, e, f, g, h, i and j, which underlies each text window. 

it is used to convey the results of numberical OSLO calculations to variables in CCL commands.

twr - textwin_reset: clear text window

sbr - ssbuf_reset: clear spreadsheet buffer and change the current row index(first argument) into row index 1 and clear the number of rows(second argument)

```
When pass the message to ssb, only numerical values are stored with full precision(14 bits) but integers and headers are not included in ssb. 
```

sbrow: return the next row that is available to be written into  

uda: update all

rin: get refractive index from surface(first argument) to surface(second argument); a column is for wavelength 1 and b column for wavelength 2 and so on...

wv[X]: get the X<sup>th</sup> wavelength value

th[X]: get the thickness value of surface X

pxt - paraxial_trace: Display the ray height, refracted angle and angle of incidence for the paraxial axial and chief rays. The default is to trace the rays in the Y-Z plane.

spd - spot_diagram: trace a spot diagram from the current object point

spd1d: display a SPD reports graphic window with all field points defined in the current system. 1D means only field points defined in the YZ planes are shown. see graph_1d2dspd.ccl

spd2d: see graph_1d2dspd.ccl
