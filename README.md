# ghostscriptwrap
# The ghostscript container to wrap ghostscript within
If the option -dSAFER is used this script uses bwrap from package bubblewrap to embbedd the final ghostscript command within a minimal container. For this a new, completely empty, filesystem namespace on a tmpfs is populate with the required libraries and files to run the final ghostscript command.
