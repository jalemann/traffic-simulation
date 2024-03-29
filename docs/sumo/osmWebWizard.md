# OSM Web Wizard for SUMO

**Warning:**  
**The OSM Web Wizard is a convenient way to select OSM Areas and convert them into SUMO net files.  
However, the OSM Web Wizard doesn't take some options into account which could be set when using `netconvert`. Netconvert and it's many options should be used for more accurate data exports whereas OSM Web Wizard can be used for more convenient exports.  
E.g. turning directions of lanes are only guessed by OSMWW**

**Convert Open Street Map data to SUMO config file**  
  
**Links**:  
[More detailed tutorial](https://sumo.dlr.de/docs/Networks/Import/OpenStreetMap.html)  
[osmWebWizard.py doc](https://sumo.dlr.de/docs/Tools/Import/OSM.html)

**How to use (tested on macOS):**
- seems to come preinstalled with SUMO
- If the macOS Application `OSM Web Wizard.app` doesn't work, use the CLI to start it
- **BUG:** Sometimes the OSM Web Wizard throws an FileNotFoundError, an easy fix is to restart the OSM Web Wizard eg. by rerunning the python command in 2
1. Find your `SUMO_HOME` dir, e.g. by looking at your `PATH` (macOS default might be `/usr/local/opt/sumo/share/sumo`)
2. Run `python3 <SUMO_HOME>/tools/osmWebWizard.py`, replacing `SUMO_HOME` according to your path
3. This will open a web tool which allows configuration for the OSM export
4. Edit preferences and click `Generate Scenario`, this will take some time then should open a SUMO window with the generated configuration
- For enhancing the generated scenario, read the [more detailed tutorial](https://sumo.dlr.de/docs/Networks/Import/OpenStreetMap.html) 
