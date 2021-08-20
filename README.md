# basetobase
Simple bash script that generates base to base conversion functions.

Conversions can be done from and to binary, octal, decimal and hexadecimal.
Also, other conversions can be handled by the script just by adding them to
the `BASES` array and to the `baseton` function.

For each base a function is created to convert given input to every
other base in the list. Each function can be called by its full name
or by a shorter three letters or a one letter version.

The naming convention is: *inputbase* to *outputbase*

ex: to convert 0x80 to decimal the three following commands can be used:
```
hexadecimaltodecimal 80
hextodec 80
htod 80
```
all of them would output: `128`

The functions use bc to execute the conversion.

To "install" the script just add the following line to your *.bashrc*:
```
[ -f ~/.basetobase ] && . ~/.basetobase
```
