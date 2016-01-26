Author(s): Itay Kruk (Mandiant, CyberHat)
           
Description:
  Antianalysis find windows api calls which recognized with anti-debugging/analysis techniques.
  Once it finds a suspicious api call it outputs the last 4 assembly instructions in order to show the function's arguments
  and help the analysts decide if this call is legitimate or not.
  


--------------------------------------------------------------------------------
How to use
--------------------------------------------------------------------------------
   Run the "antianalysis" plugin on all processes.

   ```> python vol.py -f Win2012R2x64.raw --profile=Win2012R2x64 antianalysis```

   specific process and dump pe files:

   ```> python vol.py -f Win2012R2x64.raw --profile=Win2012R2x64 antianalysis -p 1234 -D /path```
