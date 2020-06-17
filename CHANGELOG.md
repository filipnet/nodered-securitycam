# Changelog

## 2020-06-08 | BUGFIX | FATAL ERROR: Ineffective mark-compacts near heap limit Allocation failed - JavaScript heap out of memory

https://github.com/filipnet/nodered-securitycam/issues/1

## 2020-06-03 | BUGFIX | UnhandledPromiseRejectionWarning: Error: w and h must be numbers

**ISSUE:** UnhandledPromiseRejectionWarning: Error: w and h must be numbers

**SOLUTION:** The node "resize image / jimp-image" expects a numeric value of the type numbers and does not deal with the declaration of a flow variable. Entering a numeric value "400" with type "numbers" solves the error. 

## 2020-05-21 | BUGFIX | Node red crash. - JavaScript heap out of memory

**ISSUE:** Node red crash. - JavaScript heap out of memory

**SOLUTION:** Originally the buffer was written in flow variables, but with three security cameras each with 3 high-resolution photos, this has resulted in a lack of memory during processing. Therefore the code was modified, the buffer was written to a file instead of memory.
