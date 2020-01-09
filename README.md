# Freematics_CSV_Formatting
Version of Freematics firmware_v5 (https://github.com/stanleyhuangyc/Freematics) with CSV data formating.

## Usage
* Use only ./firmware_v5/telelloger folder

* Required PIDs should be defined on telelogger.ino file as follows:

  * obdData[] defines which PIDs should be **read**;
  
  * PIDLog[] defines which PIDs should be **logged**. The "pid" parameter defines the correlated PID to the current data. The "log" parameter says if the column should be created on the CSV. The "name" parameter defines the label that will be written on the CSV for the current data. Custom PIDs should be on this list.  
    * *Note that unavailable PIDs will crash the formatting. Please select to log only valid PIDs*.
    
* SHOULD_OBD_LOG and SHOULD_GPS_LOG, both on file config.h defines whether OBD and GPS data should be saved on the CSV.
