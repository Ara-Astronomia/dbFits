# What does it do?
dbFit is a script that extrapolates in batch the fitsheader from astronomical images and a gui interface (in progress)

# How to use the batch?
## on linux
open the terminal:

```bash
python ${workspace}/dbFit/src/fits.py -i $image -o $csvname > $logfile
```

## on windows
open the command prompt:

```dosbatch
python c:\%workspace%\dbFit\src\fits.py -i %image% - o %csvname%
```

sort of... (never used on windows, let me know!)

the above command creates a csv named $csvname with all the fitsheaders of the astronomical image found in directory $image
and log the operation in the log $logfile

# How to use the GUI
probabily it's useless yet :)

# Requirements

you should install python (version 2.7 or 3 should work fine!) and the python library that's responsible for reading the fitsheader: pyfits. You could install it with pip:

```bash
pip install pyfits
```

For the GUI you should install PythonCard and execute:

```bash
python ${workspace}/dbFit/src/main.py
```
