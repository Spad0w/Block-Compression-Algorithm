# Block-Model-Compression-Algorithm by Team GoldDiggers
### as part of 
### --- Software Engineering Project 2023, Semester 2 ---
- The Final Process Presentation: https://youtu.be/FuogCVHDKmM
- The Final Presentation: https://youtu.be/U1YU06rm_gk

### This project is presented as a gamified challenge which tests our design and implementation skills.
1. The task involves creating a program capable of accepting uncompressed input data through standard input and generating compressed output data via standard output without any loss of information.
2. Submit either an .exe file or a Python script for assessment by the MAPTEK verification portal: [MAPTEK TITAN](https://titan.maptek.net/).
3. The verification service will execute our code and score the submitted code based on **processing speed** and **compression performance** against all other submitted entries.

  
## Build environment

To build for **Linux** system executable:

```
make
```
## Build for Windows

To cross-compile from **Linux** to **Windows**:

```
make titan-linux
```

## Test

To see the output with the given cvs file:

```
make run
```

To time your solution:

```
make time
```



## Run semi-titan locally

To run the given py script with the created `.exe` open command prompt or powershell inside */build* folder

If you are in `wsl` directories you can use the following command and copy the build folder.

```
explorer.exe .
```

Run the test using:

```
python runner.py BLOCK11.exe the_intro_one_32768_4x4x4.csv [-r [RUNTIME]] [-s] [-v]
```


1. **-r, --runtime**: This flag specifies a minimum runtime in seconds that is used with the -s flag to improve accuracy. It can help ensure that the item under test runs for a minimum duration, allowing for more precise speed measurements. If the flag is used without specifying a value, the default is 60 seconds. If the flag is not used at all, the default value is 1000000.

2. **-s, --speed**: When this flag is present, the script will output the speed of the item under test in addition to the compression. The speed is measured relative to a reference implementation, and the output will include a floating-point number that represents the speed. Higher values are better, with 2.0 meaning twice as fast as the reference, 0.2 meaning five times slower, etc.

3. **-v, --verbose**: This flag, when present, enables more verbose output. It prints additional details and progress information to the standard error output, allowing you to see what the script is doing as it executes.
