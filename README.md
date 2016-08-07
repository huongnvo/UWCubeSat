UW CubeSat Project Main Processor Codebase
==========================================

This is the source code repository of the software system
on the main processor, based on FreeRTOS.

Build Instructions
------------------

1. Git-clone the project repository.
2. Download a copy of [TI Code Composer Studio](http://processors.wiki.ti.com/index.php/Download_CCS). Make sure you have the full/evauation license.
3. Install CCS with MSP432 libs and TI ARM compiler.
4. Import the project into CCS.

From there, you should be able to build the project sucessfully
using the Debug or Release configurations.

If you encounter a problem, it's probably due to issues with
relative paths. Contact xkxx@ and we'll figure it out.

Code Organization
-----------------

### FreeRTOS/

Source code of FreeRTOS, the embedded operating system.
Currently tracking source release v.9.0.0

DO NOT MODIFY.
When a version of FreeRTOS is released, replace the content of
this directory, but otherwise make no further changes on the
code itself.

### system/

Build config specific to the IDE. Do not modify unless you know
what you are getting into.

### dirverlib/

MSP432 low-level libraries, from TI MSP432Ware.

DO NOT MODIFY.
