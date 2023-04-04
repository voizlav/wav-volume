# Volume Control for .wav Audio Files

This is a simple C program that allows the user to modify the volume of a .wav audio file.

## Usage
To use this program, open your terminal and navigate to the directory containing the source code.

Compile the code using the following command:

```C
$ gcc -o volume volume.c

$ ./volume input.wav output.wav [FACTOR]
```

Third argument is the scaling factor to be applied to the audio data (a number greater than 0)

## How it works

This program works by reading in the header of the input .wav file, then modifying the volume of the audio data according to the scaling factor provided by the user. The modified audio data is then written to the output file.

The program assumes that the input .wav file has a standard format with a 44-byte header, and that the audio data is in the form of 16-bit signed integers.


