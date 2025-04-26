A script which will run 'sed' over all source files and replace R functions with their R_NO_REMAP equivalents.

i.e. 

1. Add `#define R_NO_REMAP` to the top of `src/*.c` files
2. Run this script to convert function names to their `NO_REMAP` equivalents  e.g. `warning()` becomes `Rf_warning()`
    * Possibly need to change the path to your `sed` executable on your system
