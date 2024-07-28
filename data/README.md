# Bell Data

These files contain raw sensor data.  The data is encoded as
lines with two fields - a timestamp, followed by a base64 encoded string.
The base64 data is sequential records from the FIFO of an LSM6dsv16x sensor mounted in a
vibration isolating mount on the headstock of the bell. 

# Groton #2
Groton files are from the #2 bell at Groton School. The y axis is more or less aligned
parallel to the bell axis, and the z axis is more or less vertical, with the bell hanging
in the down position.  The data is collected at roughly 1875 kHz, with multiple records per
sample.  Lines generally contain on the order of 32 records (IIRC).

## alderney_20240728_113355.txt

This is a quarter peal of PB Major on the back 8, with Peter B on the 10,  Greg R on the instrumented 11, John Wells (?) on the 12.
We didn't get Hawkear data for this, so there is little evidence of the striking of the other bells, except in the noise in the instrumentation signals.
The gyr_z axis is roughly the bell swing axis, xl_y is roughly vertical.
There is a short period at the end where the 11th is rung down,
swung at several heights, then rung back up.  It is hopefully
sufficient for parameter calibration.

The LSM sensor information may be found at:
https://www.st.com/resource/en/datasheet/lsm6dsv16x.pdf

Useful application notes are at:
https://www.st.com/resource/en/application_note/an5763-lsm6dsv16x-6axis-imu-with-embedded-sensor-fusion-ai-qvar-for-highend-applications-stmicroelectronics.pdf

Copies of these are also included in the datasheets directory of this repository.

