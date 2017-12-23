# OSLO
Optics Software for Layout and Optimization


# CCL notes



## Spreadsheet Buffer

it is an array of numerical storage cells with 1999 rows numbererd as in Mocrosoft Excel and 10 columns numbered as a, b c, d, e, f, g, h, i and j, which underlies each text window.

it is used to convey the results of numberical OSLO calculations to variables in CCL commands.

## Commands(Functions)

stp - set_preference: set the values of the preference given by the Preference_to_set argument.

  * outp: output_text
  * mwvl: Max_wavelengths
  * msrf: Max_surfaces
  * On/Off state

twr - textwin_reset: clear text window

sbr - ssbuf_reset: clear spreadsheet buffer and change the current row index(first argument) into row index 1 and clear the number of rows(second argument)

**When pass the message to ssb, only numerical values are stored with full precision(14 bits) but integers and headers are not included in ssb.**

sbrow: return the next row that is available to be written into  

uda: update all

rin: get refractive index from surface(first argument) to surface(second argument); a column is for wavelength 1 and b column for wavelength 2 and so on...

wv[X]: get the X<sup>th</sup> wavelength value

th[X]: get the thickness value of surface X

pxt - paraxial_trace: Display the ray height, refracted angle and angle of incidence for the paraxial axial and chief rays. The default is to trace the rays in the Y-Z plane.

sop: set object point, tracing a Hamiltonian ray which is reference ray that involve coordinates that are defied inside the lens

### Spot Diagram Evaluation commands

spd - spot_diagram: trace a spot diagram from the current object point

spd1d: display a SPD reports graphic window with all field points defined in the current system. 1D means only field points defined in the YZ planes are shown. see graph_1d2dspd.ccl

spd2d: see graph_1d2dspd.ccl

pls - plot_spot_diagram: plot single spot diagram

### Graphics window

gwo - graphwin_open: open the graphics window indicated by the numbers

gwc - graphwin_close: close the graphcis window

gwt - graphwin_title: display the string Window_title bar of the active graphics window

gwr - graphwin_reset: clear the graphics Window

#### Plot Commands

window: specify "world coordinates" to draw the window in the current viewport. (x_min, x_max, y_min, y_max)

moveto: the specified coordinates are relative to the origin of the current world coordinate system

moverel: the specified coordinates are relative to the last world coordinate point set by a previous line draing or positioning commands

lineto: the specified coordinates are relative to the origin of the current world coordinate system

linerel: the specified coordinates are relative to the last world coordinate point set by a previous line drawing or positioning commands

*The use of lineto/linerel would not change the current position of cursor. When apply moveto again, the position is still in the previous position set by previous moveto command*

label: give the labels for abscissa and ordinate axis

langle: rotate the text in clockwise

lspacing: set the speration between characters and seperation between multiple lines (each adjusted portion is 10% of the default separation). + increase and - decrease

pen: give the colour

gshow: all queued drawing requests for the current vector graphics window to be displayed immediately on the screen

```
#include "../../public/ccl/inc/gendefs.h"
```

Two commonly used graphics commands:
          - SAVE_DISPLAY_PREFS
          - RESTORE_DISPLAY_PREFS
