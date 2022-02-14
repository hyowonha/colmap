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
