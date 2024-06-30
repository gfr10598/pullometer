# Groton Data

These files contain raw sensor data from the #2 bell at Groton School.  The data is encoded as
lines with two fields - a timestamp, followed by a base64 encoded string.
The base64 data is sequential records from the FIFO of an LSM6dsv16x sensor mounted in a
vibration isolating mount on the headstock of the bell.  The y axis is more or less aligned
parallel to the bell axis, and the z axis is more or less vertical, with the bell hanging
in the down position.  The data is collected at roughly 1875 kHz, with multiple records per
sample.  Line generally contain on the order of 32 records (IIRC).

The LSM sensor information may be found at:
https://www.st.com/resource/en/datasheet/lsm6dsv16x.pdf

Useful application notes are at:
https://www.st.com/resource/en/application_note/an5763-lsm6dsv16x-6axis-imu-with-embedded-sensor-fusion-ai-qvar-for-highend-applications-stmicroelectronics.pdf

Copies of these are also included in the datasheets directory of this repository.

