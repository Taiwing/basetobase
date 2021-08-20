# basetobase
Simple bash script that generates base to base conversion functions.

Conversions from and to binary, octal, decimal and hexadecimal.

For each base a function is created to convert given input to every
other base in the list. Each function can be called by its full name
or by a shorter three letters or one letter version.

The syntax is: *inputbase*to*outputbase* number

ex: to convert 0x80 to decimal the three following commands can be used:
```
hexadecimaltodecimal 80
hextodec 80
htod 80
```
all of them would output: `128`

The functions use bc to execute the conversion.
