# osmctools
OpenStreetMap processing tools. It supports conversion between .osm, .o5m, and .pbf formats.

Sample Usage: Download and Convert .pbf to .osm
```
> gcc -o osmconvert osmconvert.c -O3 -lz
> wget http://download.geofabrik.de/asia/taiwan-latest.osm.pbf
> ./osmcomvert

osmconvert 0.8.4

Converts .osm, .o5m, .pbf, .osc, .osh files, applies changes
of .osc, .o5c, .osh files and sets limiting borders.
Use command line option -h to get a parameter overview,
or --help to get detailed help.

If you are familiar with the command line, press <Return>.

If you do not know how to operate the command line, please
enter "a" (press key E and hit <Return>).
a
-----------------------------------------------------------------
Hi, I am osmconBert - just call me Bert.
I will guide you through the basic functions of osmconvert.

At first, please ensure to have the "osmconvert" file
(resp. "osmconvert.exe" file if Windows) located in the
same directory in which all your OSM data is stored.

You may exit this program whenever you like. Just hold
the <Ctrl> key and press the key C.

Please please tell me the name of the file you want to process:
../taiwan-latest.osm.pbf
Thanks!
-----------------------------------------------------------------
What may I do with this file?

  1  convert it to a different file format
  2  use an OSM Changefile to update this file
  3  use a border box to limit the geographical region
  4  use a border polygon file to limit the geographical region
  5  minimize file size by deleting author information
  6  display statistics of the file
To options 3 or 4 you may also choose:
  a  keep ways complete, even if they cross the border
  b  keep ways and areas complete, even if they cross the border

Please enter the number of one or more functions you choose:
1
All right.
-----------------------------------------------------------------
Please choose the output file format:

1 .osm (standard XML format - results in very large files)
2 .o5m (binary format - allows fast)
3 .pbf (standard binary format - results in small files)

Enter 1, 2 or 3:
1
Thanks!
-----------------------------------------------------------------
Now, please hang on - I am working for you.
If the input file is very large, this will take several minutes.

If you want to get acquainted with the much more powerful
command line, this would have been your command:

osmconvert ../taiwan-latest.osm.pbf --out-osm -o=../taiwan-latest.osm
-----------------------------------------------------------------
-----------------------------------------------------------------
Finished! Calculation time: 9s.
I just completed your new file with this name:
  ../taiwan-latest.osm
Thanks for visiting me. Bye!
Yours, Bert
```
