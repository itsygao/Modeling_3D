# Simple 3D Modeling Program

> Gourd shape (Bezier Mode):

<img src="imgsrc/gourd_draw.png" height="360">
<img src="imgsrc/gourd_model.png" height="360">

> Plate shape (Bspline Mode):

<img src="imgsrc/plate_draw.png" height="356">
<img src="imgsrc/plate_model.png" height="356">

> With this simple 3D Modeling program, you can easily create `.obj` files by customizing curves and rotation axis. Let's see how this works!

# Step1: Run the code

> This program will run on Windows computers.
> 1. Open the `.sln` file in the folder
> 2. Click the green arrow on the top of Visual Studio (Start Without Debugging)

# Step2: Basic interaction

> At this moment, there should be 2 windows on your screen: `Curve Window` on the left and `Model Viewer` on the right.


<img src="imgsrc/start1.png">

> The left window should have one vertical white line with 2 points on it. The point in the middle (call it M) is the origin for our coordinate frame, and when combined with the other point (call it P) shows a length of 0.1.
> In short, the vector `MP` is has an absolute length of 0.1.

> Our coordinate frame is shown below in pink:

<img src="imgsrc/axis.jpg">

> The curve we draw will be rotated around the blue line (axis) and the vertices coordinates will be recorded in the pink frame.

# Step 3: Change Axis

> Don't forget the exe window. It have a lot of helpful info, but never type into this shell. Always type into `Curve Window` or `Model Viewer`.

<img src="imgsrc/start2_exewindow.png">

> My program allow users to change the rotation axis. The axis angle is defined to be the acute angle between the axis and the horizontal line. To change, go to `Curve Window`, press 'a', and enter a number between 0-90. Press 'f' to save.

<img src="imgsrc/start3_changeAxis.png">

> For example, type "a32f" will change the rotation angle to 32 degrees. See image above.

<img src="imgsrc/start3_changeAxis2.png">

> However if the number you typed is too big, it will reset your input in the middle. For example, typing "a322f" will set the angle to 2 degrees, as the program will clear the input when the second 2 is entered. See image above.

> It's highly recommended to change the axis first, before you start drawing points (though it will still work if you first draw something, then change the axis).

# Step 4: Change size

> You can use 's' to make your model smaller. The unit (0.1) length will therefore be longer. You can also use 'b' to make the model bigger and the unit length shorter on screen. Pressing 's' multiple times can allow you to change unit (0.1) vector direction, moving Point P to the other side of Point M. Here P is moved to the right side of M after ~20 presses (see the shell outputs)

<img src="imgsrc/start3_big.png">

# Step 5: Draw and generate

> It's basically the same commands as HW3. Use 0/1/2 to draw straight lines/bezier/bspline curves. Left click to add, right click to remove, drag to move.

> When you are finished, press 'g' to generate. You can find the file generated here. Filename is "my3DModel.obj".

<img src="imgsrc/start3_file.png">

> Unfortunately the `Model Viewer` will not update right now. It will update when you close the program with `q` and relaunch it.

# Step 6: Viewing

> It's basically the same commands as HW2. Please press 'h' on `Model Viewer` window for more information.

# Normal Calculation:

<img src="imgsrc/normal_calc.jpg">

# Have fun exploring!

> #to comply with UCSD academic intergrity rules, no code will be posted publicly.