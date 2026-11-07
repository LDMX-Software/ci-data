# ESA26 cosmics with ECal L1

`run298.dat.xz`: the first 100 MB (whole Rogue records) of ESA26 run 298
(07-Nov-2026, Run_298_20261107_131153.dat): HCal-triggered cosmics at ~400 Hz,
ECal L1 (ECON-D 1, ROC0-4, eRx 2, 3 off), L2, L3 and HCal, all zero suppressed,
5 samples, ECal L1OFFSET 65, L1-L3 at 100 V. L1 leveled (07-Nov calibration
set), L1 ZS at pedestal + 7 ADC. 28961 HCal events, 50 readouts with hits in
all three ECal layers.

Not used by ldmx-sw CI yet; it is meant to replace run 271 in
`esa26_cosmics_data` once ldmx-sw decodes L1 and has run-dependent ESA26
pedestals and ZS bounds.
