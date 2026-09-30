# Hyundai Elantra CN7 OBD2 PIDs

This is a list of OBD2 PIDs supported by a Hyundai Elantra CN7 MY2023 with the 1.6 MPI Smartstream engine sold in Europe.

The vehicle has been built in the Ulsan factory in South Korea so I'm assuming that these should also work for the 1.6 MPI and 1.6 LPI engine variants sold over there.

## Files

This repo only contains PID definitions:

* `CN7.csv` - custom PIDs for Torque (Android)
* `CN7.csp` - custom PIDs for Car Scanner (Android)

Torque dashboards and RaceRender gauges can be found at [HyundaiElantraCN7_TelemetryLayouts](https://github.com/gdincu/HyundaiElantraCN7_TelemetryLayouts).

These have been tested using the following setup:
<ul>
<li>Hardware</li>
        <ul>
        <li><a href="https://www.scantool.net/obdlink-lxbt/">OBDLink LX</a>
        <li><a href="https://www.scantool.net/obdlink-sx/">OBDLink SX</a>
        </ul>
<li>Software</li>
        <ul>
        <li><a href="https://play.google.com/store/apps/details?id=org.prowl.torque&hl=en&gl=US">Torque (Android)</a></li>
        <li><a href="https://play.google.com/store/apps/details?id=OCTech.Mobile.Applications.OBDLink&hl=en&gl=US">OBDLink (Android)</a></li>
        <li><a href="https://play.google.com/store/apps/details?id=com.ovz.carscanner&hl=en&gl=US">Car Scanner (Android)</a></li>
        <li><a href="https://www.scantool.net/obdwiz/">OBDwiz (Windows)</a></li>
        </ul>
</ul>

<h2> Standard PIDs (Service 01) </h2>

Please refer to https://en.wikipedia.org/wiki/OBD-II_PIDs for more details on these and the equations used for each one.

### PIDs supported [$01 - $20]

Support mask: `B63FA813`

| PID | Supported | Description&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr> |
| --- | --------- | ----------- |
| 01 | Yes | Monitor status since DTCs cleared.<br>(Includes malfunction indicator lamp (MIL),<br>status and number of DTCs, components tests,<br>DTC readiness checks) |
| 02 | No | - |
| 03 | Yes | Fuel system status |
| 04 | Yes | Calculated engine load |
| 05 | No | - |
| 06 | Yes | Short term fuel trim-Bank 1 |
| 07 | Yes | Long term fuel trim-Bank 1 |
| 08 | No | - |
| 09 | No | - |
| 0A | No | - |
| 0B | Yes | Intake manifold absolute pressure |
| 0C | Yes | Engine speed |
| 0D | Yes | Vehicle speed |
| 0E | Yes | Timing advance |
| 0F | Yes | Intake air temperature |
| 10 | Yes | Mass air flow sensor (MAF) air flow rate |
| 11 | Yes | Throttle position |
| 12 | No | - |
| 13 | Yes | Oxygen sensors present (in 2 banks) |
| 14 | No | - |
| 15 | Yes | Oxygen Sensor 2 / A: Voltage / B: Short term fuel trim |
| 16 | No | - |
| 17 | No | - |
| 18 | No | - |
| 19 | No | - |
| 1A | No | - |
| 1B | No | - |
| 1C | Yes | OBD standards this vehicle conforms to |
| 1D | No | - |
| 1E | No | - |
| 1F | Yes | Run time since engine start |
| 20 | Yes | PIDs supported [$21 - $40] |

### PIDs supported [$21 - $40]

Support mask: `801DB011`

| PID | Supported | Description&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr> |
| --- | --------- | ----------- |
| 21 | Yes | Distance traveled with malfunction indicator lamp (MIL) on |
| 22 | No | - |
| 23 | No | - |
| 24 | No | - |
| 25 | No | - |
| 26 | No | - |
| 27 | No | - |
| 28 | No | - |
| 29 | No | - |
| 2A | No | - |
| 2B | No | - |
| 2C | Yes | Commanded EGR |
| 2D | Yes | EGR Error |
| 2E | Yes | Commanded evaporative purge |
| 2F | No | - |
| 30 | Yes | Warm-ups since codes cleared |
| 31 | Yes | Distance traveled since codes cleared |
| 32 | No | - |
| 33 | Yes | Absolute Barometric Pressure |
| 34 | Yes | Oxygen Sensor 1 / AB: Air-Fuel Equivalence Ratio (lambda,λ) / CD: Current |
| 35 | No | - |
| 36 | No | - |
| 37 | No | - |
| 38 | No | - |
| 39 | No | - |
| 3A | No | - |
| 3B | No | - |
| 3C | Yes | Catalyst Temperature: Bank 1, Sensor 1 |
| 3D | No | - |
| 3E | No | - |
| 3F | No | - |
| 40 | Yes | PIDs supported [$41 - $60] |

### PIDs supported [$41 - $60]

Support mask: `FED08C05`

| PID | Supported | Description&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr> |
| --- | --------- | ----------- |
| 41 | Yes | Monitor status this drive cycle |
| 42 | Yes | Control module voltage |
| 43 | Yes | Absolute load value |
| 44 | Yes | Commanded Air-Fuel Equivalence Ratio (lambda,λ) |
| 45 | Yes | Relative throttle position |
| 46 | Yes | Ambient air temperature |
| 47 | Yes | Absolute throttle position B |
| 48 | No | - |
| 49 | Yes | Accelerator pedal position D |
| 4A | Yes | Accelerator pedal position E |
| 4B | No | - |
| 4C | Yes | Commanded throttle actuator |
| 4D | No | - |
| 4E | No | - |
| 4F | No | - |
| 50 | No | - |
| 51 | Yes | Fuel Type |
| 52 | No | - |
| 53 | No | - |
| 54 | No | - |
| 55 | Yes | Short term secondary oxygen sensor trim, A: bank 1, B: bank 3 |
| 56 | Yes | Long term secondary oxygen sensor trim, A: bank 1, B: bank 3 |
| 57 | No | - |
| 58 | No | - |
| 59 | No | - |
| 5A | No | - |
| 5B | No | - |
| 5C | No | - |
| 5D | No | - |
| 5E | Yes | Engine fuel rate |
| 5F | No | - |
| 60 | Yes | PIDs supported [$61 - $80] |

### PIDs supported [$61 - $80]

Support mask: `02000001`

| PID | Supported | Description&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr> |
| --- | --------- | ----------- |
| 61 | No | - |
| 62 | No | - |
| 63 | No | - |
| 64 | No | - |
| 65 | No | - |
| 66 | No | - |
| 67 | Yes | Engine coolant temperature |
| 68 | No | - |
| 69 | No | - |
| 6A | No | - |
| 6B | No | - |
| 6C | No | - |
| 6D | No | - |
| 6E | No | - |
| 6F | No | - |
| 70 | No | - |
| 71 | No | - |
| 72 | No | - |
| 73 | No | - |
| 74 | No | - |
| 75 | No | - |
| 76 | No | - |
| 77 | No | - |
| 78 | No | - |
| 79 | No | - |
| 7A | No | - |
| 7B | No | - |
| 7C | No | - |
| 7D | No | - |
| 7E | No | - |
| 7F | No | - |
| 80 | Yes | PIDs supported [$81 - $A0] |

### PIDs supported [$81 - $A0]

Support mask: `00000008`

| PID | Supported | Description&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr>&emsp;<wbr> |
| --- | --------- | ----------- |
| 81 | No | - |
| 82 | No | - |
| 83 | No | - |
| 84 | No | - |
| 85 | No | - |
| 86 | No | - |
| 87 | No | - |
| 88 | No | - |
| 89 | No | - |
| 8A | No | - |
| 8B | No | - |
| 8C | No | - |
| 8D | No | - |
| 8E | No | - |
| 8F | No | - |
| 90 | No | - |
| 91 | No | - |
| 92 | No | - |
| 93 | No | - |
| 94 | No | - |
| 95 | No | - |
| 96 | No | - |
| 97 | No | - |
| 98 | No | - |
| 99 | No | - |
| 9A | No | - |
| 9B | No | - |
| 9C | No | - |
| 9D | Yes | Engine Fuel Rate |
| 9E | No | - |
| 9F | No | - |
| A0 | Yes | PIDs supported [$A1 - $C0] |

    
<h2> Custom PIDs </h2>

<h3>Torque</h3>
<a href="https://github.com/gdincu/HyundaiElantraCN7-OBD2-PIDs/blob/main/CN7.csv">These</a> PIDs are setup to be used via the Torque app and therefore some of the formulas are based on the <a href="https://wiki.torque-bhp.com/view/Equations">Torque Wiki</a>.

<h3>Car Scanner</h3>
<a href="https://github.com/gdincu/HyundaiElantraCN7_OBD2_PIDs/blob/main/CN7.csp">These</a> PIDs are setup to be used via the Car Scanner app and therefore some of the formulas are based on the <a href="https://www.carscanner.info/custompids/)">Car Scanner Wiki</a>.

`CN7_Buttons.csp` is experimental / untested - action buttons that send commands to the car. Verify carefully before use.
