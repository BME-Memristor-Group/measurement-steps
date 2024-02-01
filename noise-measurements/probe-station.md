# Probe Station Measurement Steps

## Search for Conduct /w Normal Setup

1. **Prepare** the Sample
   1. With the *blue ground hand band* put the sample to the probe station's tray.
      1. The sample can be not stable, check the glue and push the sides of the sample down.
   2. **Open** the probe station's cage, and slide in the tray. Turn the fixer, so it will stay in place.
   3. Using the microscope zoomed out, put the left cantilever onto the side of the sample. **this has the channel nb. 3**
   4. **Zoom** on the sample, and put the right cantilever onto the right part which you want to measure. **this has the channel nb. 4**
      1. Be aware that the optics can be tricky about where the end of the cantilever is.
2. **Prepare** the measurement setup
   1. Use the following default order.
    Measurement Card -> Splitter -> Serial Resistance -> Probe station In (**ch. 4**) -> Probe station Out (**ch. 4**) -> Current Amplifier -> Splitter -> Measurement Card
3. **Open** LabView on the PC
   1. Open the Memristor Group Project
      1. Check in the *_Setting.vi* that
   2. Open Memristor_autosave.vi
   3. On the left side, check the parameters
      1. This default setup has a 50 Ohm bias.
   4. Select the Search Conduct Page
   5. Start the Measurement on the left top.

## IV /w Normal Setup

1. **Select** the IV panel
   1. Check the parameters (Volt, Direction, Full Swipe, Time, Nb. of Measurements)
   2. Do a test swipe (def. 0.5 V, 0.1s, full, pos.)
      1. The sample should have a linear IV curve on this spectrum
      2. If there is a recurring huge amplitude in the IV curve, your setup has some unusually high noise. Check the setup, and mitigate the noise.
   3. Do 5 swipes (on def. 1V 1s full pos) to check the stability of the sample
   4. **SET** the switch (with def. 3V, 1s, half, neg)
   5. Do 5 swipes
   6. **RESET** the switch (with def. 3V, 1s, half, pos)
   7. Do 5 swipes
