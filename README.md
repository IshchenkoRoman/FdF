# FdF
## Intoduction
The representation in 3D of a landscape is a critical aspect of modern mapping. For
example, in these times of spatial exploration, to have a 3D representation of Mars is a
prerequisite condition to its conquest. As another example, comparing various 3D representations
of an area of high tectonic activity will allow you to better understand these
phenomenon and their evolution, and as a result be better prepared.

## Objectives
In this project you will discover the basics of graphic programming, and in particular how
to place points in space, how to join them with segments and most importantly how to
observe the scene from a particular viewpoint.
You will also discover your first graphic library: **miniLibX**. This library was developed
internally and includes the minimum necessary to open a window, light a pixel and deal
with events linked to this window: keyboard and mouse. This project introduces you to
“events” programming. Don’t forget to watch the e-learning videos!

## General Instructions
 1.  The executable file named fdf.
 2.  Makefile must compile the project and must contain the usual rules. It does not recompile and re-link the program unless necessary.
 3.  This project use the **miniLibX**. Either in the version that is available on the system, or from its sources.
 4.  This project use the following functions:
     - 1) open, read, write, close
     - 2) malloc, free
     - 3) exit
     - 4) functions defined in the math library (-lm and man 3 math)
     - 5) functions defined in the **miniLibX** library.
 ## Mandatory part
 This project is about creating a simplified graphic “wireframe” (“fils de fer” in french,
hence the name of the project) representation of a relief landscape linking various points
(x, y, z) via segments. The coordinates of this landscape are stored in a file passed as
a parameter to your program. Here is an example:
```
$>cat 42.fdf
0 0 0  0  0  0  0  0  0 0 0 0  0  0  0  0  0  0 0
0 0 0  0  0  0  0  0  0 0 0 0  0  0  0  0  0  0 0
0 0 10 10 0  0  10 10 0 0 0 10 10 10 10 10 0  0 0
0 0 10 10 0  0  10 10 0 0 0 0  0  0  0  10 10 0 0
0 0 10 10 0  0  10 10 0 0 0 0  0  0  0  10 10 0 0
0 0 10 10 10 10 10 10 0 0 0 0  10 10 10 10 0  0 0
0 0 0  10 10 10 10 10 0 0 0 10 10 0  0  0  0  0 0
0 0 0  0  0  0  10 10 0 0 0 10 10 0  0  0  0  0 0
0 0 0  0  0  0  10 10 0 0 0 10 10 10 10 10 10 0 0
0 0 0  0  0  0  0  0  0 0 0 0  0  0  0  0  0  0 0
0 0 0  0  0  0  0  0  0 0 0 0  0  0  0  0  0  0 0
$>
```

**_Each number corresponds to a point in space_**
1)The horizontal position corresponds to its axis.
2)The vertical position corresponds to its ordinate.
3)The value corresponds to its altitude.

## Showtime
If you execute your program fdf on this file, we should see something like this:
```
$>./fdf 42.fdf
```

<img width="2198" alt="screen shot 2017-11-30 at 9 05 15 pm" src="https://user-images.githubusercontent.com/30857998/34018848-cf4870f2-e123-11e7-9c9d-384b5e128236.png">
<img width="2187" alt="screen shot 2017-11-30 at 9 05 35 pm" src="https://user-images.githubusercontent.com/30857998/34018926-33a27980-e124-11e7-9330-87c7515a1de6.png">
<img width="2189" alt="screen shot 2017-11-30 at 9 05 54 pm" src="https://user-images.githubusercontent.com/30857998/34018930-37056c40-e124-11e7-873f-4f736f8eaae5.png">
<img width="2191" alt="screen shot 2017-11-30 at 9 06 17 pm" src="https://user-images.githubusercontent.com/30857998/34018932-381e3f94-e124-11e7-916a-2e8cd4cf30f6.png">

