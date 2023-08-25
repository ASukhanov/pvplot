# pvplot
Plotting tool for EPICS PVs, ADO and LITE parameters.

![Stripchart example](docs/pvplot_stripchart.png)

![Example of an array plot](docs/pvplot_arrays.png)

## Examples
- Sliced array plot of an EPICS PV: ```pvplot -a'E:testAPD:scope1:' 'Waveform_RBV[1:500]'```
- Strip chart of analog inputs of a LabJack U3-HV instrument, served by liteLabjack:
pvplot -a'L:localhost:dev1' 'tempU3 ADC_HV[0] ADC_HV[1] ADC_HV[2] ADC_HV[3] ADC_LV'
- Fast correlation plot of litePeakSimulator ```pvplot -s.01 -a'L:localhost:dev1' 'x,y'```
- To change properties of curves: right click on a plot and select 'DataSets Options'
#TODO:- Two plots, correlation and two-curve stripchart: ```pvplot -#0'simple.test:sinM,am_simple.0:sinM' -#1'simple.test:sinM am_simple.0:sinM'```

