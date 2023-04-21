# BMS-charge-control
simple node red flow to dynamically control managed battery charging

This is a fairly simple node red flow to manage a controlled battery (BMS)
This includes dashboard inputs to set the bulk/abs voltage values, and max charge amps.
It will also poll the BMS for min and max cell voltages and display them on the dashboard with the cell id number, the cell deviation, and battery temp.
after you load the flow into node red, you will need to set the victron nodes to match your system.
Change the default settings injection to match your system. You can also change the dashboard input nodes to set the min/max values for your system.
lastly, change the values in the calculation function node to meet your requirements. The function includes arguments to produce a stepped charging current based on voltage.
I have added notes to the flow to try to make it as simple of a setup as possible.

Use at your own risk. I assume no responsibility if your system suddenly launches to the moon.
