# ghostscriptwrap
## The ghostscript container to wrap ghostscript within
If the option -dSAFER is used this script uses bwrap from package bubblewrap to embbedd the final ghostscript command within a minimal container. For this a new, completely empty, filesystem namespace on a tmpfs is populate with the required libraries and files to run the final ghostscript command.

To install the bash script gswrap you have to change the line

    ghostscript=@@GS@@

in this script to the full path of your ghostscript binary.
