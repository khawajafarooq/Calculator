# AutoLayoutCalculatorUI

Autolayout is a powerful feature to build resizeable dynamic user interface for iOS platform. But it comes with the great complexity to tackle so many constraints for a laying out multiple views on the screen. It's super handy to use *Stack View* to tackle with this complexity. **Stack View** is a user control that allows to layout views in a stack in either horizontal or vertical orientation.

For the sake of ease, I have build a demonstration of calculator application user interface using stack views and autolayouts.


**Steps to follow:**

1. Create a single view project
2. Add a label on view controller and embed it inside a stack view using *Editor > Embed In > Stack view or button at the bottom*
![Alt text](/screenshots/al1.jpg?raw=true "Embed inside stack view")

3. Now add 20 buttons (5 rows, 4 columns)
![Alt text](/screenshots/al2.jpg?raw=true "Buttons grid")

4. Insert each row of buttons inside a stack view. You can also name the stack view for identification
![Alt text](/screenshots/al3.jpg?raw=true "Inser each buttons row inside a stack view")

5. Select all the stack views and embed them inside another stack view which we will call **Root Stack View**. Now we have stack of stacks
![Alt text](/screenshots/al4.jpg?raw=true "Root Stack View")

6. Select Root Stack View and then add 4 constraints for top, left, bottom, right to standard values which is zero (0).
![Alt text](/screenshots/al5.jpg?raw=true "Adding constraint")

7. Perform following for Root Stack View:
  - Set the alignment of Root Stack View Fill
  - Set spacing for Root Stack View to 8 px iOS standard
  - Set Distribution to Fill Equally
8. Repeat step 7 for all child stack views. Yes, you are almost there!
![Alt text](/screenshots/al6.jpg?raw=true "Almost there!")

9. Looks like there is a small warning left by autolayout. Fix it by selecting the warning and update frames for it.
![Alt text](/screenshots/al7.jpg?raw=true "Fixing one last warning")

Now the calculator layout is ready to use. It works smooth across all the screen sizes and orientations.

There are other ways to achieve this but I have done this using stack views. Stack views are super easy to learn. I recommend you should give a try!
