# pvplot
Plotting tool for EPICS PVs, ADO and LITE parameters.

![Stripchart example](docs/pvplot_stripchart.png)

![Example of an array plot](docs/pvplot_arrays.png)

## Examples
- Correlation plot sinM vs degM: ```pvplot 'simple.test:degM,simple.test:sinM'```
- Stripchart plot for two PVs: ```pvplot 'simple.test:sinM am_simple.0:sinM'```
- Two plots, correlation and two-curve stripchart: ```pvplot -#0'simple.test:sinM,am_simple.0:sinM' -#1'simple.test:sinM am_simple.0:sinM'```
- Sliced array plot of an EPICS PV: ```pvplot 'E:testAPD:scope1:Waveform_RBV[1:500]'```
- Fast plotting of a LiteServer parameter:  ```pvplot L:acnlin23:dev1:y -s.001```
- Datasets options: right click on a plot and select 'DataSets Options'
- Legends can be added by enabling Legend checkbox after right click.
