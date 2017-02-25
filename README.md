# AutoLayoutCalculatorUI

Autolayout is a powerful feature to build resizeable dynamic user interface for iOS platform. But it comes with the great complexity to tackle so many constraints for a laying out multiple views on the screen. It's super handy to use **Stack Views** to tackle with this complexity.

For the sake of ease, I have build a demonstration of calculator application user interface using stack views and autolayouts.


**Steps to follow:**

1. Create a single view application project
2. Add a label on view controller and embed it inside a stack view using *Editor > Embed In > Stack view or button at the bottom*

![Alt text](/screenshots/al1.png?raw=true "Embed inside stack view")

3. Now add 20 buttons (5 rows, 4 columns)
![Alt text](/screenshots/al2.png?raw=true "Embed inside stack view")

4. Insert each row of buttons inside a stack view. You can also name the stack view for identification
![Alt text](/screenshots/al3.png?raw=true "Embed inside stack view")

5. Select all the stack views and embed them inside another stack view which we will call **Root Stack View**
![Alt text](/screenshots/al4.png?raw=true "Embed inside stack view")

6. Select Root Stack View and then add 4 constraints for top, left, bottom, right to standard values which is zero (0).
![Alt text](/screenshots/al5.png?raw=true "Embed inside stack view")

7. Perform following for Root Stack View:
  - Set the alignment of Root Stack View Fill
  - Set spacing for Root Stack View to 8 px iOS standard
  - Set Distribution to Fill Equally
8. Repease step 7 for all child stack views. This will pretty much set your layout user interface
![Alt text](/screenshots/al6.png?raw=true "Embed inside stack view")

9. Looks like there is a still small warning left by autolayout. Fix it by selecting the warning and press fix misplacement for the option update frames.
![Alt text](/screenshots/al7.png?raw=true "Embed inside stack view")

Now your layout will be smooth and ready for all the screen size and orientations.

There are other ways to achieve this but I have done this using stack views. Stack views are super easy to learn. I recommend you should give a try!
