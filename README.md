# egeoONE
Example library to use the tools of the eGEO ONE hardware platform

JSON Structure
{
  "operation": "Desired operation(String)",
  "d1": "data1 (16bit Unsigned integer)",
  "d2": "data2 (16bit Unsigned integer)",
  "d3": "data3 (Double precision floating point DBL)",
  "msgl1": (String 16 Characters)
  "msgl2": (String 16 Characters) 
}

RESPONSE:
{"value":"Response(integer, double or String)"}

OPERATIONS:

Get Meter ID: {"operation":"getID"}

Get Temperature: {"operation":"getTemp"}
     
Get Phase A Power: {"operation":"getPowerA"}

Get Phase B Power: {"operation":"Open getPowerB"}

Get Phase C Power:  {"operation":"getPowerC"}

Get Total Power: {"operation":"getPowerT"}

Get Phase A Reactive Power: {"operation":"getQPowerA"}

Get Phase B Reactive Power: {"operation":"getQPowerB"}

Get Phase C Reactive Power: {"operation":"getQPowerC"}

Get Total Reactive Power: {"operation":"getQPowerT"}

Get Fundamental Harmonic Power of Phase A: {"operation":"getPmeanAF"}

Get Fundamental Harmonic Power of Phase B: {"operation":"getPmeanBF"}

Get Fundamental Harmonic Power of Phase C: {"operation":"getPmeanCF"}
      
Get Total Fundamental Harmonic Power: {"operation":"getPmeanTF"}

Get Harmonic Power Phase A: {"operation":"getPmeanAH"}

Get Harmonic Power Phase B: {"operation":"getPmeanBH"}

Get Harmonic Power Phase C: {"operation":"getPmeanCH"}

Get Total Harmonic Power: {"operation":"getPmeanTH"}

Get RMS Voltage Phase A: {"operation":"getVoltageA"}

Get RMS Current Phase A: {"operation":"getCurrentA"}

Get RMS Voltage Phase B: {"operation":"getVoltageB"}

Get RMS Current Phase B: {"operation":"getCurrentB"}

Get RMS Voltage Phase C: {"operation":"getVoltageC"}

Get RMS Current Phase C: {"operation":"getCurrentC"}
     
Get RMS Current Phase N: {"operation":"getCurrentN"}

Get Frequency: {"operation":"getFrequency"}

Get Total Power Factor: {"operation":"getPFT"}

Get Phase A Power Factor: {"operation":"getPFA"}

Get Phase B Power Factor: {"operation":"getPFB"}

Get Phase C Power Factor:: {"operation":"getPFC"}

Get State of Phase A Relay: {"operation":"getRelayA"}

Disconnect Phase A Relay: {"operation":"disconnectPowerA"}

Connect Phase A Relay: {"operation":"connectPowerA"}

Get State of Phase B&C Relay: {"operation":"getRelayBC"}

Disconnect Phase B&C Relay: {"operation":"disconnectPowerBC"}

Connect Phase B&C Relay: {"operation":"connectPowerBC"}

Get Acumulated Active Energy: {"operation":"getTDAE"}

Get Acumulated Inverse Active Energy: {"operation":"getTIAE"}
      
Get Acumulated Reactive Energy: {"operation":"getTDRE"}
        
Get Acumulated Inverse Reactive Energy: {"operation":"getTIRE"}

Set Date: {"operation":"setDate", "d1":UNIX date}
      
Set Connection State in Display: {"operation":"setOnline"}

Send Message Via Display(5Sec): {"operation": "setDisplay", "msgl1": (Line 1 String 16 Characters) "msgl2": (Line 2 String 16 Characters)}
      
Reboot Metering Chipset: {"operation":"reboot"} 
