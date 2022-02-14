SfM-focused COLMAP
======

About
-----

This is a dieted version of COLMAP (https://github.com/colmap/colmap) with removed parts that are too miscellaneous or unrelated to SfM, to help beginners get to the core SfM algorithms directly and intuitively.

The entry point to the main program is in `src/main.cc`.

How to compile
-----

```
mkdir build
cd build
cmake .. -DCMAKE_BUILD_TYPE=Release -G Ninja
ninja
```

How to run
-----

```
# Command line mode
./colmap sfm --image_path /path/to/image/folder 
             --workspace_path /path/to/store/database 
             (optional args)

# GUI mode
./colmap gui
```


License
-----

Please be mindful that this repository was forked from the original COLMAP. All of the original license for COLMAP and those for its dependencies must be kept.
Below is the original COLMAP's license.
```
Copyright (c) 2022, ETH Zurich and UNC Chapel Hill.
All rights reserved.

Redistribution and use in source and binary forms, with or without
modification, are permitted provided that the following conditions are met:

    * Redistributions of source code must retain the above copyright
      notice, this list of conditions and the following disclaimer.

    * Redistributions in binary form must reproduce the above copyright
      notice, this list of conditions and the following disclaimer in the
      documentation and/or other materials provided with the distribution.

    * Neither the name of ETH Zurich and UNC Chapel Hill nor the names of
      its contributors may be used to endorse or promote products derived
      from this software without specific prior written permission.

THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDERS OR CONTRIBUTORS BE
LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR
CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF
SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN
CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
POSSIBILITY OF SUCH DAMAGE.

Author: Johannes L. Schoenberger (jsch-at-demuc-dot-de)
```
