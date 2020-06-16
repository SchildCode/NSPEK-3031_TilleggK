# NSPEK-3031_TilleggK
- Simulation of hourly heat pump performance with with macro-enabled bilinear interpolation of capacity and COP in accordance with European standards EN 13612-2, EN 14825, and Norwegian Technical Specification SN NSPEK 3031:2020 Tillegg K (Appendix K).
- The workbook also calculates part-load COP using a relation between Part-Load Factor (PLF) vs Part-Load Ratio (PLR). This is done in a flexible way that can handle any heat pump (both single-speed and variable-speed compressors for air/air, air/water, water/air or water/water heat pumps). This approach is an improvement upon EN 13612-2, EN 14825, but still compliant by adjusting the 3 coefficients.
- The workbook is partly in Norwegian.
- The workbook contains four example sheets (with red-colourd tabs) for hourly heat-pump calculations. In each case the calculations integrate the total energy delivered to the heat pump and the electric boiler:
  1. Space heating only
  2. Domestic hot water production only
  3. Simultaneous production of space heating and domestic hot water from the same primary circuit 
  4. Heat pump with shunt-valve to switch between producing high-temperature heat to domestic hot water, and low-temperature heat to space heating
- The worksheet does not calculate pump energy. You can easily modify the spreadsheet to estimate hourly total pump energy.
- In addition, the workbook has four precalculation sheets (green-coloured tabs) that may be used to generate input data for pasting into the (red) heat pump calclation sheets:
  1. Visualization of part load profiles (PLR vs PLF), basically in complaince with EN 13612-2 and EN 14825.
  2. Generating one year of hourly loads (space+ventilation heating, and domestic hot water), and separate generation of hourly setpoint temperature for the supply to the hydronic heating system based on an outdoor-temperature compensation curve.
  3. An example table for Ground Source Heat Pump (GSHP) typical COP and capacity tables as a function of condenser and evapourator water temperatures. The whole capacity table can be automatically recalculated from one user-specified capacity [W]
  4. Calculation of hourly borehole outlet temperature for a whole year, in accordance with the simple cosine curve and tabulated values given in European Standard EN 15450.

### Licence & warranty
- Provided under the GPL3 licence.
- It is provided with no warranty of any kind.

### Author
- peter.schild@OsloMet.no
