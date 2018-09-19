# tiepatch
Patcher for TIE Corps patching system (remake of 16bit ZT patcher)

## Notes
* Written using Delphi Embaracdero RAD Studio XE2 by Colonel Impulse
* Forked as a backup to the eh-tac repository

## Bytemap file format
* The first 12 bytes are the filename in 8.3 format
* Next byte is always 00
* Next two bytes are the number of records
* Each record is 6 bytes - 4 byte offset in the destination file, then 1 byte for the number of bytes to replace, then the replacement
* EH patches are always 1 byte replacements.
* Filename is in big endian byte order, everything else is little endian
