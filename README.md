# OSLO
Optics Software for Layout and Optimization


CCL notes

- Spreadsheet Buffer
it is an array of numerical storage cells with 1999 rows numbererd as in Mocrosoft Excel and 10 columns numbered as a, b c, d, e, f, g, h, i and j, which underlies each text window. 
it is used to convey the results of numberical OSLO calculations to variables in CCL commands.

twr - textwin_reset: clear text window
sbr - ssbuf_reset: clear spreadsheet buffer and change the current row index(first argument) into row index 1 and clear the number of rows(second argument)

When pass the message to ssb, only numerical values are stored with full precision(14 bits) but integers and headers are not included in ssb. 

sbrow: return the next row that is available to be written into  
