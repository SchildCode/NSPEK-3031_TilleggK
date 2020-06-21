# NSPEK-3031_TilleggK
- Simulation of hourly performance of heat-pumps or chillers by means of bilinear interpolation of capacity and COP in accordance with International standards ISO 13612-2 <sup>[[2]](#2)</sup>, EN 14825 <sup>[[2]](#2)</sup>, and Appendix K of Norwegian Technical Specification SN NSPEK 3031:2020 <sup>[[1]](#1)</sup>.
- The workbook also calculates part-load COP using a relation between Part-Load Factor (PLF) vs Part-Load Ratio (PLR). This is done in a flexible way that can handle all kinds of heat pump (both single-speed and variable-speed compressors for air/air, air/water, water/air or water/water heat pumps). This approach is documented in two papers <sup>[[4]](#4)[[5]](#5)</sup>, and is an improvement upon EN 13612-2, EN 14825, but still compliant by adjusting the 3 coefficients.

- The workbook contains four example sheets (with red-colourd tabs) for hourly heat-pump calculations. In each case the calculations integrate the total energy delivered to the heat pump and the electric boiler:
  1. Space heating only
  2. Domestic hot water production only
  3. Simultaneous production of space heating and domestic hot water from the same primary circuit 
  4. Heat pump with shunt-valve to switch between producing high-temperature heat to domestic hot water, and low-temperature heat to space heating
- In addition, the workbook has four precalculation sheets (green-coloured tabs) that may be used to generate input data for pasting into the (red) heat pump calclation sheets:
  1. Visualization of part load profiles (PLR vs PLF) using equations documented in scientific papers [[6]](#6) & [[7]](#7), and in complaince with ISO 13612-2 and EN 14825.
  2. Generating a year of hourly loads (space+ventilation heating, and domestic hot water) based in a very simple hourly dynamic model similar to that given in ISO 13790 <sup>[[3]](#3)</sup>, and separate generation of hourly setpoint temperature for the supply to the hydronic heating system based on an outdoor-temperature compensation curve.
  3. An example table for Ground Source Heat Pump (GSHP) typical COP and capacity tables as a function of condenser and evapourator water temperatures, calculated as a median of the data tabulated by multiple manufacturers. The whole capacity table can be automatically recalculated from one user-specified capacity [W]
  4. Calculation of hourly borehole outlet temperature for a whole year, in accordance with the simple cosine curve and tabulated values given in European Standard EN 15450 <sup>[[5]](#5)</sup>.
- Caveats:
  1. The workbook is partly in Norwegian.
  2. The worksheet does not calculate energy for circulation pumps. However, it is easy to modify the spreadsheet to summate hourly energy for circulation pumps by using pump laws, similar to that used by e.g. https://product-selection.grundfos.com/.


### Licence & warranty
- Provided under the GPL3 licence.
- It is provided with no warranty of any kind.

### Author
- peter.schild@OsloMet.no

### References cited above
- <a id="1">[1]</a> SN-NSPEK 3031:2020: <i>"Energy performance of buildings — Calculation of energy needs and energy supply"</i> (In Norwegian)
- <a id="2">[2]</a> ISO 13612-2: <i>"Heating and cooling systems in buildings — Method for calculation of the system performance and system design for heat pump systems — Part 2: Energy calculation"</i>
- <a id="3">[3]</a> ISO 13790: <i>"Thermal performance of buildings - Calculation of energy use for space heating"</i> (Withdrawn)
- <a id="4">[4]</a> EN 14825: <i>"Air conditioners, liquid chilling packages and heat pumps, with electrically driven compressors, for space heating and cooling — Testing and rating at part load conditions and calculation of seasonal performance"</i>
- <a id="5">[5]</a> EN 15450: <i>"Heating systems in buildings - Design of heat pump heating systems"</i>
- <a id="6">[6]</a> Fuentes, E., Waddicor, D., Fannan, M. O., & Salom, J. (2017). "Improved methodology for testing the part load performance of water-to-water heat pumps". In <i>Proceedings of 12th IEA Heat Pump Conference 2017</i>.
- <a id="7">[7]</a> Henderson, H. I., Parker, D., & Huang, Y. J. (2000). "Improving DOE-2's RESYS routine: User defined functions to provide more accurate part load energy use and humidity predictions". In <i>Proceedings of 2000 ACEEE Summer Study on Energy Efficiency in Buildings, August 20-25, 2000, Pacific Grove, CA</i>



